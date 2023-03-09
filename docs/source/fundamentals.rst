Fundamentals
==============

Erigon is different from many other implementations of Ethereum (or other blockchain protocols) being less monolithic and more *modular*. But the word "modular" here needs to be understood quite specifically.

Modules are not just code packages that end up complied into a single executable. In Erigon, modules (or "components") are parts of Erigon that can be taken out into a separate executable, and then operated in its own process (of the operating system), or even on its own computer in the network.

Below is the illustration of how Erigon currently splits up into components (modules):

img
<img title="Erigon architecture" alt="Erigon architecture" src="https://substackcdn.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2Fa2de43fb-457e-4691-86bb-c655d8c3c48b_607x581.png">


