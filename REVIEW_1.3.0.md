# Independent review — 1.3.0-alpha
## Improvements
- Win rate denominator now counts only closed trades, not open positions.
- Dashboard separates wins, losses, open positions and recorded net P/L.
- Numeric fields use a decimal keyboard and basic validation.
- Outcome entry rejects zero and sign-inconsistent P/L (WIN positive; LOSS negative).
- Version metadata and release notes updated.

## Remaining critical limitations
- Position size semantics are not yet defined (base units, quote notional, or margin); therefore automatic P/L is intentionally not fabricated.
- Entry 1/2 and TP/SL are stored as user inputs; weighted average entry, partial exits and fee/funding calculations are not implemented.
- P/L is user-entered, not exchange-verified.
- No edit flow, backup/restore, CSV export, or automated UI tests yet.
- Build/install not executed in an Android runtime here.
