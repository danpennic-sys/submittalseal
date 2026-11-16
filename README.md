# SubmittalSeal

**Local-first construction submittal, shop drawing, product data, and approval evidence sealer for field operators.**

Offline. Deterministic. Pay once. Compatible with QuantumGuard CONTRACT-v1 and the Operator Pages suite.

## Why SubmittalSeal?

Rejected or disputed submittals, missing shop drawing approvals, and "we never received that product data" claims delay projects and create claims. Without a contemporaneous, verifiable record of what was submitted, by whom, to whom, with what attachments (hashes), and what the response was, defense and payment fail.

SubmittalSeal captures structured submittal records (type, spec section, description, submitter, recipient, status, response, media hashes) and seals them into a client-verifiable QuantumGuard evidence bundle.

- No SaaS. No subscription. Runs completely offline after key setup.
- Clients, owners, or auditors verify with free QuantumGuard verifier (`qg verify`).
- Deterministic: same inputs → same sealed pack.
- Pairs with ChangeOrderSeal, DailySeal, PermitSeal, MaterialSeal, and the rest of the Operator Pages suite.

## Quick Start

```bash
pip install cryptography

python3 src/submittalseal.py --demo
python3 src/submittalseal.py --json samples/submittal-001.json --out sealed-submittal.json
```

Verify:
```bash
qg verify sealed-submittal.json
```
Expected: **PASS**.

## What you can sell

| SKU       | Price | Includes                                      |
|-----------|-------|-----------------------------------------------|
| Operator  | $69   | CLI + sample templates + key setup guide + 1-year email support |
| Command   | $189  | + batch mode + CSV/HTML export + reseller rights |
| Agency    | $479  | + white-label + multi-site key management |

**Contact:** danpennic@gmail.com for production checkout links.  
Repo: https://github.com/danpennic-sys/submittalseal

Source free under Apache-2.0 OR MIT. Commercial packs sold separately.

## License

Apache-2.0 OR MIT
