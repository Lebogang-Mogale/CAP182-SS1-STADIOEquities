# The following non-target features are created:

| Feature | Description |
|---|---|
| `BalancePerProduct` | Balance divided by number of products, using a safe denominator. |
| `AgeBand` | 18–29, 30–39, 40–49, 50–59, 60+. |
| `TenureBand` | 0–2, 3–5, 6–8 and 9–10 years. |
| `CreditScoreBand` | <580, 580–669, 670–739, 740–799, 800+. |
| `IsBalanceZero` | 1 when Balance equals zero; otherwise 0. |

The Exited target is never used to construct features.

**Implementation:** notebooks/02_Feature_Engineering.ipynb.
