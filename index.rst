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

Once you are accustomed to the basics, we recommend you read the `Solidity by Example <https://test-api-v2.readthedocs.io/en/latest/solidity-by-example.html>`
to understand the core concepts of the language.



**2. TWAMM Backend**

Time-Weighted Average Market Maker (TWAMM) is a new on-chain automated market making model designed by 
Paradigm researchers Dave White, Dan Robinson, and Uniswap founder Hayden Adams. TWAMM allows market 
participants to efficiently execute large orders on multiple blocks of Ethereum and works by breaking longterm large orders
 down into an infinite number of infinitely small virtual orders, and executing transactions smoothly over time using an embedded AMM.
 Pulsar develops the first TWAMM smart contract that integrates the DAO buyback and DEX trading. We refer `TWAMM Design Principles <https://www.paradigm.xyz/2021/07/twamm/>`_ 
 and `TWAMM Mathematical Formulation <https://hackmd.io/@luffy/SJxSsOH1Y>`_ for more information.

**3. Term Swap**
Pulsar provides "Term Swap" as its core functionality for DAO buyback and DEX trading. Traders can submit 
"LongTerm Orders" to Pulsar's TWAMM protocol to sell a fixed number of assets on a fixed number of blocks.
The benefit of Term Swap over Instant Swap (e.g. Uniswap) the flexibility in controlling the trading time, hence results in a lower slippage cost.



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
   :caption: Core API

   introduction-to-smart-contracts.rst
   installing-solidity.rst
   .. solidity-by-example.rst

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
