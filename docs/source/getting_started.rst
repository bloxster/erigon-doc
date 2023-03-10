
Getting started
===============

In order to use Erigon, the software must first be installed. There are several ways Erigon can be installed depending on the operating system and the user's choice of installation method, for example using a package manager, container or building from source.

System Requirements
--------------------

For an Archive node of Ethereum Mainnet it is recommended >=3TB storage space: 1.8TB state (as of March 2022), 200GB temp files (can symlink or mount folder <datadir>/temp to another disk).

- Ethereum Mainnet Full node ( see --prune* flags): 400Gb (April 2022).
- Goerli Full node (see --prune* flags): 189GB on Beta, 114GB on Alpha (April 2022).
- Gnosis Chain Archive: 370GB (January 2023).
- BSC Archive: 7TB. BSC Full: 1TB.
- Polygon Mainnet Archive: 5TB. Polygon Mumbai Archive: 1TB.

As a storage mean, it is reccomended to have SSD or NVMe disk. HDD is not reccomended because it will cause Erigon to always stay *N* blocks behind chain tip, but not fall behind. Furthermore, SSD performance deteriorates when close to capacity. 🔬 more details on disk storage `here <https://erigon.substack.com/p/disk-footprint-changes-in-new-erigon?s=r>`_ and `here <https://ledgerwatch.github.io/turbo_geth_release.html#Disk-space>`_.

CPU: 64-bit architecture

RAM: ≥16GB

On Linux: kernel > v4

`Golang version <https://go.dev/doc/install>`_ ≥ 1.18; `GCC <https://go.dev/doc/install/gccgo>`_ 10+ or `Clang <https://clang.llvm.org>`_



Installing Erigon
-------------------

For building the latest stable release (this will be suitable for most users just wanting to run a node):


``git clone --branch stable --single-branch https://github.com/ledgerwatch/erigon.git

cd erigon

make erigon``

You can check the `list of releases <https://github.com/ledgerwatch/erigon/releases>`_ for release notes.

For building the bleeding edge development branch:

``git clone --recurse-submodules https://github.com/ledgerwatch/erigon.git
cd erigon
git checkout devel
make erigon``
