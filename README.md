Original fork of Bitcoin 0.3. Chain was forked to alpha-node (Bitcoin 0.27) in Sep 24. 

If you need to migrate your coins mined on this chain build the code and use alphacash --printkeys
This will print out the private keys into a file called keys.dat
Then use bx ec-to-wif --uncompressed KEY to convert to uncompressed wif format
then use alpha-cli to importprivkey KEY to import into an alpha wallet.


********************************************************************************************************************

Abstract: Alphacash is a censorship resistant peer-to-peer electronic cash system. Similar to Bitcoin, it uses a fixed emission schedule and longest chain Proof of Work consensus protocol. Unlike Bitcoin, it supports unlimited blocksize with a multi-machine horizontally scaling architecture, without sacrificing security or censorship resistance. The Alphacash coins replicate the self-verifiability property of physical cash, i.e. the coins are compact, authenticated data structures which can be passed through any medium peer-to-peer, chain-to-chain and verified without bridges or trusted third parties. Alphacash completes the Bitcoin vision, functioning as an Internet currency, a medium of exchange and a genuine alternative to physical cash.


The initial code is a minimalist version of Bitcoin PoW forked from 0.3 

The key change is in the transaction validation code - transactions are only valid if they have single input. 

                size_t no_of_inputs = vin.size();
                if (no_of_inputs > 1)
                    return false;
                    
Coinbase maturity 120 blocks

Genesis Block "Financial Times 25/May/2024 What went wrong with capitalism"











