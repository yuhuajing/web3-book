#  Web3 Development Book

## Useful Links
1. This book is hosted on GitHub: <https://github.com/yuhuajing/web3-book>
2. Page in <>

## Table of Contents
- Milestone 0. Solidity Data
  1. data-bytes
  2. data-enum
  3. data-foreach
  4. data-mapping
  5. data-variables
  6. data-encode
- Milestone 1. Solidity functions
  1. variables-slot-storage
  2. variables-unicode
  3. variables-user-defined-type
- Milestone 2. Solidity variables
  1. Functions
  2. Functions modifier
  3. Functions selector
  4. Functions sendValue
  5. errors check
- Milestone 3. Sollidity contracts create
  1. contracts-import
  2. contracts-create
  3. contracts-creationcodes
  4. contracts-destroy
  5. contracts-event
  6. contracts-getcodes
- Milestone 4: Sollidity contracts type
  1. contracts-interface
  2. contracts-library
  3. contracts-abstract
  4. contracts-inherite
  5. contracts-proxy
- Milestone 5. Sollidity contracts call
  1. contracts-call
  2. contracts-delegatecall
  3. contrats-staticcall
  4. contracts-precompile
- Milestone 6. Sollidity advanced
  1. merkle tree
  2. ecdsa signature
## Running locally

To run the book locally:
1. Install [Rust](https://www.rust-lang.org/).
1. Install [mdBook](https://github.com/rust-lang/mdBook):
    ```shell
    $ cargo install mdbook
    $ cargo install mdbook-katex
    ```
1. Clone the repo:
    ```shell
    $ git clone https://github.com/yuhuajing/solidity-book.git
    $ cd solidity-book
    ```
1. Run:
    ```shell
    $ mdbook serve --open
    ```
1. Visit http://localhost:3000/ (or whatever URL the previous command outputs!)
