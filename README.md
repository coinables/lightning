# lightning

`cli/lightning-cli help` will output a list of available lightning-cli commands. 

##### dev-blockheight
  - Show current block height
##### dev-setfees
  - Set feerate in satoshi-per-kw for {immediate}, {normal} and {slow} (each is optional, when set, separate by spaces) and show the value of those three feerates
##### listnodes
  - Show all nodes in our local network view
##### getroute
  - Show route to {id} for {msatoshi}, using {riskfactor} and optional {cltv} (default 9)
##### listchannels
  - Show all known channels
##### invoice
  - Create an invoice for {msatoshi} with {label} and {description} with optional {expiry} seconds (default 1 hour)
##### listinvoice
  - (DEPRECATED) Show invoice {label} (or all, if no {label}))
##### listinvoices
  - Show invoice {label} (or all, if no {label})
##### delinvoice
  - Delete unpaid invoice {label} with {status}
##### waitanyinvoice
  - Wait for the next invoice to be paid, after {lastpay_index} (if supplied)
##### waitinvoice
  - Wait for an incoming payment matching the invoice with {label}
##### decodepay
  - Decode {bolt11}, using {description} if necessary
##### help
  - Show available commands
##### stop
  - Shut down the lightningd process
##### getlog
  - Show logs, with optional log {level} (info|unusual|debug|io)
##### dev-rhash
  - Show SHA256 of {secret}
##### dev-crash
  - Crash lightningd by calling fatal()
##### getinfo
  - Show information about this node
##### sendpay
  - Send along {route} in return for preimage of {rhash}
##### pay
  - Send payment specified by {bolt11} with optional {msatoshi} (if and only if {bolt11} does not have amount), {description} (required if {bolt11} uses description hash) and {riskfactor} (default 1.0)
##### listpayments
  - Show outgoing payments
##### connect
  - Connect to {id} at {host} (which can end in ':port' if not default)
##### listpeers
  - Show current peers, if {level} is set, include {log}s
##### fundchannel
  - Fund channel with {id} using {satoshi} satoshis
##### close
  - Close the channel with peer {id}
##### dev-sign-last-tx
  - Sign and show the last commitment transaction with peer {id}
##### dev-fail
  - Fail with peer {id}
##### dev-reenable-commit
  - Re-enable the commit timer on peer {id}
##### dev-ping
  - Send {peerid} a ping of length {len} asking for {pongbytes}
##### dev-memdump
  - Show memory objects currently in use
##### dev-memleak
  - Show unreferenced memory objects
##### withdraw
  - Send to {destination} address {satoshi} (or 'all') amount via Bitcoin transaction
##### newaddr
  - Get a new address to fund a channel
##### listfunds
  - Show funds available for opening channels
