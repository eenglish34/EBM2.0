Eblockmail - Port: 3434 RPC Port: 3435

Specs
  Type: Masternode/POS
  Reward Split: 70% MN / 30% POS
  Block Time: 60 Seconds
  Confirmations: 15
  Masternode Confirmations: 15
  Minimum coins required for staking: 100
  POS Maturity Time: 2 hours
  Total Coin Supply: 500,000,000
  Pre mine: 10,000,000


Linux Compiling Instruction
  ./autogen.sh
  ./configure --disable-tests --disable-bench
  make

when done
  strip ./eblockmaild
  strip ./eblockmail-cli
