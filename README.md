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

If asked to mine, vault-proto looks for the key as set with rpc call setminingkey [privkey]

To create N units in the next coinbase, use rpccall setissuenextblock [amount]   

Current status:  Demo in progress



