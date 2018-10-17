# Towards Improved Plasma Constructions

All in one explanatory paper on Plasma Cash, featuring reference implementation at https://github.com/loomnetwork/plasma-cash


## Protocols
- Deposit coin (either through approve-transfer for erc20/erc721 or with erc721 receiver)
- Send coin (offchain)
- Verify coin received protocol
- Exit
- Challenge Types, exit period windows etc.
- Withdrawal protocol 

## Functionalities
- Proof of Inclusion / Exclusion (optimized with default bitfield for SMTS)
- Signing a transaction
- Cryptoeconomic bonds to ensure valid behavior

## Attacks
- Block Withholding
- Griefing (constant factor? unlimited?)

## Future work
- Arbitrary denomination payments
  - Plasma Debit analysis
  - Plasma Defragmentation/Cashflow
  - Fast withdrawals
  - Proofs / formalization (maybe in this paper?)

# Compiling/Editing
`make`. Cleanup repo with `make clean`

## Generating figures
Requires dia

```
cd figures
python dia2pdf.py
```

## Formatting

80 character width by default.
There are a couple places where reflowing will break (primarily in figures where it's sensitive to linebreaks).
