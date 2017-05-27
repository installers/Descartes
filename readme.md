  bankonmeOS source code builder version 4 It has been decided that each and every release of the bankonmeOS developer edition will proceed along using the English alphabet where the last name of a famous philosopher is in the release title. Charles Babbage did his part to make the mechanical computer a reality. Noam Chompsky explored new ways of categorizing language. Descartes concluded that the only thing he could not doubt was himslelf with the classic "Cogito Ergo Sum". Of course I learned a little more about bash this round... and added the first if/then statement for user interaction. Tested on a fresh install of Ubuntu 16.04LTS amd64.

  The bankonmeOS project goal is simple... "to protect cryptocurrency from malice or unintentional use".

Shortening the name of the install file to bankonme.mag and will continue this policy. Version four updates include adding the Bytecoin and Exodus Wallets. Zcash, Electrum, Litecoin-core, Bitcoin-core, Namecoin-core, Dashcore and Bitsquare are still included. Bitsquare is a decentralized cryptocurrency exchange platform. Electrum is useful for cold storage and offline use. Exodus is a wallet that includes Shapeshift code. Read the documentation a few times. I will be re-reading the documentation myself. (see docs.electrum.org)

I am releasing what may be the first .mag file into the wild. *.mag files are an extension released under the MIT license. *.mag (c) 2011,2012,2013,2014,2015,2016,2017 Gregory L. Magnusson MIT license

I used to program PHP in .mag files.... then I found bash.

... this build takes a while and requires a 64 bit machine, 2 gig of ram (at least) and 200 gigs of space to be safe. The blockchains are growing. Pure genius created the code and the code is pure genius.

##########################################

To generate a source build of Bitcoin-Core, Namecoin-Core, Litecoin-Core, Dash, Electrum, Exodus, Bytecoin and Armory just copy and paste the following into a bash terminal as one line

$ sudo apt-get update && sudo apt-get upgrade -y && sudo apt-get install git -y && git clone https://github.com/bankonmeOS/Descartes.git && cd Descartes && chmod +x bankonme.mag && sudo ./bankonme.mag

##########################################

you can http://bankon.me

Building from these cryptocurrency wallets from source takes a while (hours on an i5). With a test on an i7 laptop expect an instance of Bitcoin-Core and Dashcoin-Core within the hour. Downloading the blockchains takes even longer. By longer I am referring to downloading almost 200 gigabytes which could take hours, days or weeks depending on your computer and network access speeds. The permissions seem adequate installing from source as root produces ownership at 0644 where users can load instances of the wallet from the terminal for exampe $ /usr/local/bin/bitcoin-qt

Subsequent instances of the wallets can be started as a regular user for instance

$ /usr/local/bin/litecoin-qt &

A production use binary build script is in the works as the "chomsky" project found at https://github.com/bankonmeOS/chomsky 
This is the developer edition. 

If you have a ton of cryptocurrency you need a computer that is NOT connected to the Internet and create a paper wallet and put that paper in a safe or safe place. Lose the passphrase lose the value. I am proving that as I chase down 3.0 Zcash that I picked up in the early days. Really!!! Web Wallets are not safe for long term storage of any amount you consider to be moderate value. Binary build coming soon. Bitsquare, the decentralized cyrptocurrency exchange has been added as a binary. In the future Bitsquare will be a source build with the developer edition and a binary build with the production edition. Recent experiments have shown that a binary build co-exists effortlessly with a source build on the same hard drive.

Graphics will be added to each of the source built wallets for ease of use....

Subseqent boot regular user wallet startup

Bitcoin

$/usr/local/bin/bitcoin-qt &

Litecoin

$/usr/local/bin/litecoin-qt &

Dashcoin

$/usr/local/bin/dash-qt

Namecoin

$/usr/local/bin/namecoin-qt &

Bitsquare (start from menu)

Applications --> Other --> Bitsquare

Armory (start from menu)

Applications --> Internet --> Armory

###

Bytecoin startup can be done from the menu Applications --> Office --> Bytecoin
Bitsquare startup can be done from the menu Applications --> Other --> Bitsquare
. I will be making menu tabs for the other wallets.

This is a great paper wallet creator written in Javascript

https://github.com/bankonmeOS/WalletGenerator.net

Have fun out there on the client side.

note: the build will take several hours and your computer will grind for a while. Downloading the blockchains will take between hours, days, and a week. It took me 72 hours to download the Bitcoin blockchain on the last test. In the future I will try to allow for a choice of wallets instead of the current plethora. In the mean time more wallets are being added.
