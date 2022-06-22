Pulsar
========

`Pulsar <https://pulsarswap.com/>`_ is a decentralized platform that provides joint functionalities on a decentralized exchange center (DEX) and the buyback of DAO shares.
In particular, we offer DEX consisting of both instant swap and term swap. The term swap enables trades with long-term orders with lower slippage costs. It also offers
the buyback of DAO shares with the purchase time window is completely set at users' discretion.  


This documentation details the APIs we offer at Pulsar for two purposes:

* Provide instruction for DAO buybacks on how to submit the buyback order.
* Provide instruction for customers who participate in the buyback or related trades.



When deploying contracts, you should use the latest released
version of Solidity. Apart from exceptional cases, only the latest version receives
`security fixes <https://github.com/ethereum/solidity/security/policy#supported-versions>`_.
Furthermore, breaking changes as well as
new features are introduced regularly. We currently use
a 0.y.z version number `to indicate this fast pace of change <https://semver.org/#spec-item-4>`_.

.. warning::

  Solidity recently released the 0.8.x version that introduced a lot of breaking
  changes. Make sure you read :doc:`the full list <080-breaking-changes>`.

Ideas for improving Solidity or this documentation are always welcome,
read our :doc:`contributors guide <contributing>` for more details.

.. Hint::

  You can download this documentation as PDF, HTML or Epub by clicking on the versions
  flyout menu in the bottom-left corner and selecting the preferred download format.


Getting Started
---------------
Here we introduce some preliminaries.

**1. Get to Know Solidity**

Solidity is a `curly-bracket language <https://en.wikipedia.org/wiki/List_of_programming_languages_by_type#Curly-bracket_languages>`_ designed to target the Ethereum Virtual Machine (EVM).
It is influenced by C++, Python and JavaScript. You can find more details about which languages Solidity has been inspired by in the :doc:`language influences <language-influences>` section.

Solidity is statically typed, supports inheritance, libraries and complex
user-defined types among other features.

With Solidity you can create contracts for uses such as voting, crowdfunding, blind auctions,
and multi-signature wallets.

Once you are accustomed to the basics, we recommend you read the :doc:`"Solidity by Example" <solidity-by-example>`
and “Language Description” sections to understand the core concepts of the language.



**2. Term Swap**

There are various ways to install the Solidity compiler,
simply choose your preferred option and follow the steps outlined on the :ref:`installation page <installing-solidity>`.

.. hint::
  You can try out code examples directly in your browser with the
  `Remix IDE <https://remix.ethereum.org>`_. Remix is a web browser based IDE
  that allows you to write, deploy and administer Solidity smart contracts, without
  the need to install Solidity locally.

.. warning::
    As humans write software, it can have bugs. You should follow established
    software development best-practices when writing your smart contracts. This
    includes code review, testing, audits, and correctness proofs. Smart contract
    users are sometimes more confident with code than their authors, and
    blockchains and smart contracts have their own unique issues to
    watch out for, so before working on production code, make sure you read the
    :ref:`security_considerations` section.

**4. Learn More**

If you want to learn more about this project Pulsar, we refer `Pulsar Official Website <https://pulsarswap.com/>`_ for details.
`Ethereum Developer Resources <https://ethereum.org/en/developers/>`_
can help you with further general documentation around Ethereum, and a wide selection of tutorials,
tools and development frameworks.


Contents
========

:ref:`Keyword Index <genindex>`, :ref:`Search Page <search>`

.. toctree::
   :maxdepth: 2
   :caption: Basics

   introduction-to-smart-contracts.rst
   installing-solidity.rst
   solidity-by-example.rst

.. toctree::
   :maxdepth: 2
   :caption: Language Description

   layout-of-source-files.rst
   structure-of-a-contract.rst
   types.rst
   units-and-global-variables.rst
   control-structures.rst
   contracts.rst
   assembly.rst
   cheatsheet.rst
   grammar.rst

.. toctree::
   :maxdepth: 2
   :caption: Compiler

   using-the-compiler.rst
   analysing-compilation-output.rst
   ir-breaking-changes.rst

.. toctree::
   :maxdepth: 2
   :caption: Internals

   internals/layout_in_storage.rst
   internals/layout_in_memory.rst
   internals/layout_in_calldata.rst
   internals/variable_cleanup.rst
   internals/source_mappings.rst
   internals/optimizer.rst
   metadata.rst
   abi-spec.rst

.. toctree::
   :maxdepth: 2
   :caption: Additional Material

   050-breaking-changes.rst
   060-breaking-changes.rst
   070-breaking-changes.rst
   080-breaking-changes.rst
   natspec-format.rst
   security-considerations.rst
   smtchecker.rst
   resources.rst
   path-resolution.rst
   yul.rst
   style-guide.rst
   common-patterns.rst
   bugs.rst
   contributing.rst
   brand-guide.rst
   language-influences.rst
