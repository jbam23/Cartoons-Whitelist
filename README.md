# Cartoons-Whitelist

Cartoons Contract Address: 0xeE29700134AAB4f45b113E43E29ff06ce10687b7

Text file contains 3818 Whitelisted addresses for Cartoons NFT. Search for your address in the text file to see if it is whitelisted.

With the attached proof you will have all the data needed to whitelist mint from contract.

Under "Read Contract" in Cartoons contract, function #4 getAllowedMintAmount will return the number of whitelist mints avaiable for an address. The first input is the
bytes32 proof from the attached text file (copy everything inside the quotation marks, should look like a long list 0x123,0x234,0x567 when you input it into etherscan), and
the second is the user address whose proof you are checking. This will return the amount of mints that address has from the whitelist.

TO WHITELIST MINT: Under "Write Contract" in Cartoons contract, function #16 whitelistMint allows a whitelisted address to mint using their proof.
First input is the amount of ether (0.07 per mint, so 0.07 for 1 and 0.14 for 2), second input is the proof found in the text file (remember to exclude the quotations), and the third input is the amount to mint (Must be less or equal to the allocated whitelist amount, initially set to 2).
