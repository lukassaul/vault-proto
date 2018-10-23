Vault Prototype integration/staging tree
=====================================

Keyed Mining Coin
----------------

Vault-proto an experimental digital currency that enables instant payments to
anyone, anywhere in the world. Vault-proto uses peer-to-peer technology to operate
with a central authority: managing transactions is carried
out collectively by the network while issuing currency is carried out by keyed computers, where
keys are issued by a central authoridy.  Coin redemption is to be handled solely by the company 
in control of the mining keys.  

The block chain is fully auditablle and visible by all participants; this is a public coin in all aspects, 
it is only the issuance itself which is semi-private - the issuance events are all publicly visible for complete transparency of operations.  

Otherwise the network behaves exactly as Litecoin Core, enabled for segwit and all the other bells and whistles.

Type 1 Vault addresses begin with a V  

Block time is 30 seconds.  

For prototype the genesis block is kept as the litecoin block.  


New RPC Calls
----------------

Two new RPC calls area added for keyed miningg operation:  

If asked to mine with rpc call "setgenerate true", 
vault-proto looks for the key as set with rpc call setminingkey [privkey].  If no valid key is present, mining will continue but no block will ever be found.  

To create N units in the next coinbase, use rpccall setissuenextblock [amount]   No limit to issuance in this version, but all events are public and visible on the block chain.  

Current status:  Demo in progress


Fees
----------------

Fees are set to 0.1% of each transaction.  Miners get the fees as usual, but now miners must have a key to produce a block, so keyed miners collect all fees.  



