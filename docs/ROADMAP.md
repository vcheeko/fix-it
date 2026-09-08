# Fix-it roadmap

Status: proposed work; no completion dates or runtime results are claimed.

## 1. Public concept

Document purpose, scope, current limitations and the relationship to Korako. This repository provides that initial documentation.

## 2. Digital-task accounting simulation

Implement a local test ledger using synthetic identities and test balances, without real funds or provider credentials.

Minimum records: job ID, quote ID and expiry, approved maximum, accounting unit, reservation, measured usage, verification result, settlement and refund entries.

Acceptance criteria:
- Reject unapproved or expired quotes and insufficient balance.
- Reserve only the approved amount.
- Never settle more than the authorized limit.
- Keep execution, verification and payment states separate.
- Release unused reservations.
- Define cancellation, failure and refund behavior.
- Replayed requests and callbacks cannot charge twice.
- Recover consistently after interruption at each financial transition.
- Concurrent requests cannot overspend one balance.
- Disputed work enters review rather than silently becoming accepted.
- Every balance change reconciles to an auditable entry.

Publish only reproducible synthetic evidence after implementation and review.

## 3. Bounded Korako integration

Connect one real digital workflow to the simulated ledger. Record provider usage where available, distinguish estimates from measured costs and provide a human-readable receipt.

Acceptance: useful output, explicit budget approval, verification and reproducible accounting. Passing simulation does not establish readiness to handle money.

## 4. Payment-partner pilot

Select supported currencies, suitable partners and a bounded operating region. Define net payouts, fees, custody responsibilities, reconciliation, refunds and complaint handling before using real funds.

Acceptance requires the relevant operational and jurisdictional reviews, actual partner arrangements and end-to-end settlement evidence.

## 5. Local service and community pilot

Start with one service category and verified providers. Establish job standards, inspection, disputes and separately accounted assistance contributions.

Measure completion quality, response time, complaints, remediation cost and participant experience. Do not invent time savings or treat star ratings as safety certification.

## 6. Cryptocurrency decision and prototype

Document why a Fix-it token improves the validated service. Evaluate transferability, custody, liquidity, costs and legal classification. Define the design before choosing a chain.

If justified, build and review a testnet prototype. No token launch or token sale is authorized by this roadmap.

## 7. Expansion

Expand only where payment connections, qualified providers, support and protection mechanisms work. Treat each additional project, territory and service category as a distinct readiness decision.

NEXST remains a separate research track and is not a prerequisite.

## Reporting discipline

For each milestone publish scope, artifact or commit, test method, result, limitations and unresolved issues. Label planned, implemented, tested and independently verified work separately.
