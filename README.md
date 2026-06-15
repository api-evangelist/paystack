# Paystack (paystack)

Paystack is an African payment processor (acquired by Stripe in 2020) that lets businesses accept payments in Nigeria, Ghana, South Africa, Kenya, Côte d'Ivoire, and Egypt across cards, bank transfers, USSD, QR, EFT, and mobile money channels. Its single REST API covers one-time charges, recurring subscriptions, marketplace splits, dedicated virtual accounts, invoices, transfers (payouts), refunds, disputes, settlements, and KYC/identity verification — all wrapped in a developer experience that has made it one of the most respected public APIs on the continent.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/paystack/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/paystack/main/apis.yml)

## Scope

- **Position:** Consuming
- **Access:** 3rd-Party

## Tags

- Payments
- Africa
- Fintech
- Recurring Billing
- Marketplaces
- Payouts
- Mobile Money
- Stripe

## Timestamps

- **Created:** 2026-05-24
- **Modified:** 2026-05-30

## APIs

### Paystack Accept Payments API

Initialize, verify, charge, and manage one-time card, bank, USSD, mobile money, QR, and bank transfer payments. The Transaction and Charge resources are the core of Paystack — a hosted checkout flow (initialize + verify) and a direct charge flow that drives the customer through PIN, OTP, phone, birthday, and address challenges as required.

- **Human URL:** [https://paystack.com/docs/api/transaction/](https://paystack.com/docs/api/transaction/)

#### Tags

- Payments
- Transactions
- Charge

#### Properties

- [Documentation](https://paystack.com/docs/api/transaction/)
- [Documentation](https://paystack.com/docs/api/charge/)
- [OpenAPI](openapi/paystack-accept-payments-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/paystack-accept-payments.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/paystack-accept-payments.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/paystack-transaction-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/paystack-transaction-structure.json)
- [Example](examples/paystack-initialize-transaction-example.json)
- [Example](examples/paystack-verify-transaction-example.json)

### Paystack Subscriptions API

Create plans and run recurring subscriptions against stored card authorizations. Includes plan management, subscription lifecycle (create / disable / enable), customer self-service update links, and automatic invoice notifications.

- **Human URL:** [https://paystack.com/docs/api/subscription/](https://paystack.com/docs/api/subscription/)

#### Tags

- Recurring Billing
- Subscriptions
- Plans

#### Properties

- [Documentation](https://paystack.com/docs/api/subscription/)
- [Documentation](https://paystack.com/docs/api/plan/)
- [OpenAPI](openapi/paystack-subscriptions-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/paystack-subscriptions.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/paystack-subscriptions.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/paystack-plan-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/paystack-subscription-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/paystack-subscription-structure.json)
- [Example](examples/paystack-create-subscription-example.json)

### Paystack Customers API

Create, list, and update customer profiles; whitelist or blacklist customers via risk_action; deactivate stored authorizations; and run KYC validation against customer identities.

- **Human URL:** [https://paystack.com/docs/api/customer/](https://paystack.com/docs/api/customer/)

#### Tags

- Customers
- KYC

#### Properties

- [Documentation](https://paystack.com/docs/api/customer/)
- [OpenAPI](openapi/paystack-customers-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/paystack-customers.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/paystack-customers.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/paystack-customer-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/paystack-customer-structure.json)

### Paystack Transfers API

Send money out of your Paystack balance to bank accounts and mobile money wallets across supported markets. Covers transfer recipients, single and bulk transfers, OTP workflows, and bulk charges against stored authorizations.

- **Human URL:** [https://paystack.com/docs/api/transfer/](https://paystack.com/docs/api/transfer/)

#### Tags

- Payouts
- Transfers
- Bulk

#### Properties

- [Documentation](https://paystack.com/docs/api/transfer/)
- [Documentation](https://paystack.com/docs/api/transfer-recipient/)
- [Documentation](https://paystack.com/docs/api/bulk-charge/)
- [OpenAPI](openapi/paystack-transfers-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/paystack-transfers.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/paystack-transfers.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/paystack-transfer-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/paystack-transfer-structure.json)
- [Example](examples/paystack-initiate-transfer-example.json)

### Paystack Splits and Subaccounts API

Build marketplaces by automatically splitting a single payment between the main account and multiple subaccounts. Configure percentage or flat splits, set fee-bearers, and manage subaccount business profiles for vendor payouts.

- **Human URL:** [https://paystack.com/docs/api/split/](https://paystack.com/docs/api/split/)

#### Tags

- Marketplaces
- Splits
- Subaccounts

#### Properties

- [Documentation](https://paystack.com/docs/api/split/)
- [Documentation](https://paystack.com/docs/api/subaccount/)
- [OpenAPI](openapi/paystack-splits-subaccounts-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/paystack-splits-subaccounts.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/paystack-splits-subaccounts.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/paystack-split-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/paystack-subaccount-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/paystack-split-structure.json)
- [Example](examples/paystack-create-split-example.json)

### Paystack Dedicated Virtual Accounts API

Provision dedicated NUBAN virtual bank accounts for individual customers so they can pay by bank transfer with automatic reconciliation back to the customer profile. Includes split routing on inbound transfers.

- **Human URL:** [https://paystack.com/docs/api/dedicated-virtual-account/](https://paystack.com/docs/api/dedicated-virtual-account/)

#### Tags

- Bank Transfer
- NUBAN
- Virtual Accounts

#### Properties

- [Documentation](https://paystack.com/docs/api/dedicated-virtual-account/)
- [OpenAPI](openapi/paystack-dedicated-virtual-accounts-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/paystack-dedicated-virtual-accounts.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/paystack-dedicated-virtual-accounts.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Example](examples/paystack-create-dedicated-account-example.json)

### Paystack Products and Payment Pages API

Manage products in your Paystack inventory and assemble them into Paystack-hosted Payment Pages so you can collect payments without operating your own checkout.

- **Human URL:** [https://paystack.com/docs/api/products/](https://paystack.com/docs/api/products/)

#### Tags

- Hosted Checkout
- Products
- Pages

#### Properties

- [Documentation](https://paystack.com/docs/api/products/)
- [Documentation](https://paystack.com/docs/api/page/)
- [OpenAPI](openapi/paystack-products-pages-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/paystack-products-pages.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/paystack-products-pages.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Paystack Payment Requests API

Issue invoice-style payment requests to customers by email, with verification, notification, finalization, and archival flows.

- **Human URL:** [https://paystack.com/docs/api/payment-request/](https://paystack.com/docs/api/payment-request/)

#### Tags

- Invoices
- Payment Requests

#### Properties

- [Documentation](https://paystack.com/docs/api/payment-request/)
- [OpenAPI](openapi/paystack-payment-requests-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/paystack-payment-requests.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/paystack-payment-requests.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Paystack Refunds and Disputes API

Process partial and full refunds against successful transactions and respond to cardholder disputes — including evidence upload via signed URL, resolution workflows, and exports.

- **Human URL:** [https://paystack.com/docs/api/refund/](https://paystack.com/docs/api/refund/)

#### Tags

- Refunds
- Disputes
- Chargebacks

#### Properties

- [Documentation](https://paystack.com/docs/api/refund/)
- [Documentation](https://paystack.com/docs/api/dispute/)
- [OpenAPI](openapi/paystack-refunds-disputes-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/paystack-refunds-disputes.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/paystack-refunds-disputes.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/paystack-refund-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/paystack-dispute-schema.json) — [JSON Schema](https://json-schema.org/specification)

### Paystack Settlements API

Fetch settlement records and the underlying transactions that comprise each payout to your bank account.

- **Human URL:** [https://paystack.com/docs/api/settlement/](https://paystack.com/docs/api/settlement/)

#### Tags

- Settlements
- Treasury

#### Properties

- [Documentation](https://paystack.com/docs/api/settlement/)
- [OpenAPI](openapi/paystack-settlements-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/paystack-settlements.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/paystack-settlements.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Paystack Verification API

Identity, BVN, bank account, card BIN, country, bank, and address-verification lookups used to validate customers, beneficiary accounts, and cards before transacting.

- **Human URL:** [https://paystack.com/docs/api/verification/](https://paystack.com/docs/api/verification/)

#### Tags

- Verification
- Identity
- BVN
- KYC

#### Properties

- [Documentation](https://paystack.com/docs/api/verification/)
- [OpenAPI](openapi/paystack-verification-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/paystack-verification.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/paystack-verification.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Paystack Balance API

Fetch your Paystack balance per currency and read the balance ledger for treasury operations and reconciliation.

- **Human URL:** [https://paystack.com/docs/api/balance/](https://paystack.com/docs/api/balance/)

#### Tags

- Balance
- Ledger
- Treasury

#### Properties

- [Documentation](https://paystack.com/docs/api/balance/)
- [OpenAPI](openapi/paystack-balance-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/paystack-balance.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/paystack-balance.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Paystack Integration Settings API

Read and update integration-wide settings such as the payment session timeout for hosted checkout.

- **Human URL:** [https://paystack.com/docs/api/integration/](https://paystack.com/docs/api/integration/)

#### Tags

- Integration
- Settings

#### Properties

- [Documentation](https://paystack.com/docs/api/integration/)
- [OpenAPI](openapi/paystack-integration-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/paystack-integration.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/paystack-integration.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Paystack Webhooks

Outbound webhook surface that notifies a single merchant-configured POST endpoint of transaction, dispute, refund, transfer, subscription, invoice, payment request, customer identification, and dedicated virtual account events. Every delivery is signed with an HMAC-SHA512 x-paystack-signature header keyed by the merchant secret key, and Paystack retries non-200 responses for up to 72 hours.

- **Human URL:** [https://paystack.com/docs/payments/webhooks/](https://paystack.com/docs/payments/webhooks/)

#### Tags

- Webhooks
- Events
- AsyncAPI
- HMAC

#### Properties

- [Documentation](https://paystack.com/docs/payments/webhooks/)
- [AsyncAPI](asyncapi/paystack-webhooks-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)
- [Postman Collection](collections/paystack-accept-payments.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/paystack-accept-payments.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/paystack-balance.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/paystack-balance.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/paystack-customers.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/paystack-customers.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/paystack-dedicated-virtual-accounts.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/paystack-dedicated-virtual-accounts.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/paystack-integration.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/paystack-integration.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/paystack-payment-requests.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/paystack-payment-requests.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/paystack-products-pages.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/paystack-products-pages.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/paystack-refunds-disputes.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/paystack-refunds-disputes.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/paystack-settlements.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/paystack-settlements.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/paystack-splits-subaccounts.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/paystack-splits-subaccounts.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/paystack-subscriptions.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/paystack-subscriptions.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/paystack-transfers.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/paystack-transfers.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/paystack-verification.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/paystack-verification.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Arazzo Workflows](arazzo/) — [Arazzo Specification](https://spec.openapis.org/arazzo/latest.html)
- [Portal](https://paystack.com/)
- [Documentation](https://paystack.com/docs/)
- [API Reference](https://paystack.com/docs/api/)
- [Documentation](https://github.com/PaystackHQ/openapi)
- [Getting Started](https://paystack.com/docs/payments/accept-payments/)
- [Sign Up](https://dashboard.paystack.com/#/signup)
- [Documentation](https://dashboard.paystack.com/)
- [Authentication](https://paystack.com/docs/api/#authentication)
- [Documentation](https://dashboard.paystack.com/#/settings/developers)
- [Documentation](https://paystack.com/docs/payments/webhooks/)
- [Documentation](https://paystack.com/docs/payments/test-payments/)
- [Documentation](https://paystack.com/docs/api/errors/)
- [Changelog](https://paystack.com/docs/changelog/api/)
- [Blog](https://paystack.com/blog/)
- [Blog](https://medium.com/paystack-engineering)
- [Status Page](https://status.paystack.com/)
- [Support](https://support.paystack.com/)
- [Pricing](https://paystack.com/ng/pricing)
- [Pricing](https://paystack.com/gh/pricing)
- [Pricing](https://paystack.com/za/pricing)
- [Pricing](https://paystack.com/ke/pricing)
- [Pricing](https://paystack.com/ci/pricing)
- [Pricing](https://paystack.com/eg/pricing)
- [Terms of Service](https://paystack.com/terms)
- [Privacy Policy](https://paystack.com/privacy)
- [Trust Center](https://paystack.com/security)
- [GitHub Organization](https://github.com/PaystackHQ)
- [SDK](https://github.com/PaystackHQ/paystack-php)
- [SDK](https://github.com/PaystackHQ/paystack-android)
- [SDK](https://github.com/PaystackHQ/paystack-ios)
- [SDK](https://github.com/PaystackHQ/paystack-sdk-ios)
- [SDK](https://github.com/PaystackHQ/omnipay-paystack)
- [Plugins](https://github.com/PaystackHQ/plugin-woocommerce)
- [Plugins](https://github.com/PaystackHQ/plugin-magento-2)
- [Plugins](https://github.com/PaystackHQ/plugin-prestashop-1.7)
- [Plugins](https://github.com/PaystackHQ/plugin-opencart)
- [Plugins](https://github.com/PaystackHQ/plugin-whmcs)
- [Plugins](https://github.com/PaystackHQ/moodle-enrol_paystack)
- [Plugins](https://github.com/PaystackHQ/plugin-odoo)
- [Code Examples](https://github.com/PaystackHQ/PaystackJS-Sample-code)
- [Code Examples](https://github.com/PaystackHQ/sample-charge-card-backend)
- [Spectral Rules](rules/paystack-rules.yml)
- [Vocabulary](vocabulary/paystack-vocabulary.yml)
- [JSON-LD](json-ld/paystack-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Plans](plans/paystack-plans-pricing.yml)
- [Rate Limits](rate-limits/paystack-rate-limits.yml)
- [Fin Ops](finops/paystack-finops.yml)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)
- [Solutions](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
**URL:** https://apievangelist.com
