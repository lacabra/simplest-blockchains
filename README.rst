simplest-blockchain
===================

This repository is a compilation of very simple implementations in Python of a 
blockchain for educational purposes. 

You can run any of these blockchain code examples directly with the Python 
interpreter:

.. code:: bash

	$ python blockchain.v1.py

Overview
~~~~~~~~



+------------------------------------------------+-------------+-------------------------+----------------------+-------------+
| Name                                           | Lines       |Features                 | Limitations          |Requirements |
|                                                | of Code     |                         |                      |             |
+================================================+=============+=========================+======================+=============+
| `blockchain.v1.py <README.rst#blockchain-v1>`_ |     55      | * Concept of blockchain | * Single node, no p2p| None        |
|                                                |             | * Hashing               | * No mining          |             |
|		                                 |	       |                         | * No consensus       |             |
+------------------------------------------------+-------------+-------------------------+----------------------+-------------+							 

.. _blockchain-v1:

blockchain.v1.py
~~~~~~~~~~~~~~~~

Simplest implementation of all, introduces the notion of blockchain as a chain 
of blocks (locally stored in an array) and the concept of hashing. There is one 
single node that generates a first set of 20 blocks at once, and prints them 
out. It's worth noticing that when you run this same script multiple times, you 
always get different hashes for the same block in the chain, despite the fact 
that the blocks are generated in a deterministic manner. Why? Because the hash 
includes the timestamp of each block, which is always different from the last 
time you run the same script.


Credit: `aunyks <https://gist.github.com/aunyks>`_ and his original 
`Medium article <https://medium.com/crypto-currently/lets-build-the-tiniest-blockchain-e70965a248b>`_, 
and `JohnStuartRutledge <https://gist.github.com/JohnStuartRutledge>`_ for the 
Python3 version

