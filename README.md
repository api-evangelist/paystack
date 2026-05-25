# Paystack (paystack)

Paystack is an African payment processor (acquired by Stripe in 2020) that lets businesses accept payments in Nigeria, Ghana, South Africa, Kenya, Côte d'Ivoire, and Egypt across cards, bank transfers, USSD, QR, EFT, and mobile money channels. Its single REST API covers one-time charges, recurring subscriptions, marketplace splits, dedicated virtual accounts, invoices, transfers (payouts), refunds, disputes, settlements, and KYC/identity verification — all wrapped in a developer experience that has made it one of the most respected public APIs on the continent.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

- Payments, Africa, Fintech, Recurring Billing, Marketplaces, Payouts, Mobile Money, Stripe

## Timestamps

- **Created:** 2026-05-24
- **Modified:** 2026-05-24

## Markets

| Country | Currency | Local Channels |
|---|---|---|
| Nigeria | NGN | Card, Bank, USSD, QR, Bank Transfer, Apple Pay, Visa QR |
| Ghana | GHS | Card, Mobile Money (MTN, Vodafone, AirtelTigo) |
| South Africa | ZAR | Card, Instant EFT, Capitec Pay |
| Kenya | KES | M-Pesa STK Push, Card |
| Côte d'Ivoire | XOF | Orange Money, MTN MoMo, Wave, Card |
| Egypt | EGP | Card, Meeza, Fawry, Wallets |

## APIs

### Paystack Accept Payments API
Initialize, verify, charge, and manage one-time card, bank, USSD, mobile money, QR, and bank transfer payments. Covers both hosted-checkout (initialize + verify) and direct-charge flows with PIN, OTP, phone, birthday, and address challenges.

**Human URL:** [https://paystack.com/docs/api/transaction/](https://paystack.com/docs/api/transaction/)

- [Documentation — Transaction](https://paystack.com/docs/api/transaction/)
- [Documentation — Charge](https://paystack.com/docs/api/charge/)
- [OpenAPI](openapi/paystack-accept-payments-openapi.yml)
- [JSON Schema — Transaction](json-schema/paystack-transaction-schema.json)
- [JSON Structure — Transaction](json-structure/paystack-transaction-structure.json)
- [Example — Initialize Transaction](examples/paystack-initialize-transaction-example.json)
- [Example — Verify Transaction](examples/paystack-verify-transaction-example.json)
- [Naftiko Capability — Accept Payments](capabilities/accept-payments.yaml)

### Paystack Subscriptions API
Create plans and run recurring subscriptions against stored card authorizations. Includes plan management, subscription lifecycle (create / disable / enable), customer self-service update links, and automatic invoice notifications.

**Human URL:** [https://paystack.com/docs/api/subscription/](https://paystack.com/docs/api/subscription/)

- [Documentation — Subscription](https://paystack.com/docs/api/subscription/)
- [Documentation — Plan](https://paystack.com/docs/api/plan/)
- [OpenAPI](openapi/paystack-subscriptions-openapi.yml)
- [JSON Schema — Plan](json-schema/paystack-plan-schema.json)
- [JSON Schema — Subscription](json-schema/paystack-subscription-schema.json)
- [JSON Structure — Subscription](json-structure/paystack-subscription-structure.json)
- [Example — Create Subscription](examples/paystack-create-subscription-example.json)
- [Naftiko Capability — Subscriptions](capabilities/subscriptions.yaml)

### Paystack Customers API
Create, list, and update customer profiles; whitelist or blacklist customers via `risk_action`; deactivate stored authorizations; and run KYC validation.

**Human URL:** [https://paystack.com/docs/api/customer/](https://paystack.com/docs/api/customer/)

- [OpenAPI](openapi/paystack-customers-openapi.yml)
- [JSON Schema — Customer](json-schema/paystack-customer-schema.json)
- [JSON Structure — Customer](json-structure/paystack-customer-structure.json)
- [Naftiko Capability — Customers](capabilities/customers.yaml)

### Paystack Transfers API
Send money out of your Paystack balance to bank accounts and mobile money wallets across supported markets. Covers transfer recipients, single and bulk transfers, OTP workflows, and bulk charges.

**Human URL:** [https://paystack.com/docs/api/transfer/](https://paystack.com/docs/api/transfer/)

- [Documentation — Transfer](https://paystack.com/docs/api/transfer/)
- [Documentation — Transfer Recipient](https://paystack.com/docs/api/transfer-recipient/)
- [Documentation — Bulk Charge](https://paystack.com/docs/api/bulk-charge/)
- [OpenAPI](openapi/paystack-transfers-openapi.yml)
- [JSON Schema — Transfer](json-schema/paystack-transfer-schema.json)
- [JSON Structure — Transfer](json-structure/paystack-transfer-structure.json)
- [Example — Initiate Transfer](examples/paystack-initiate-transfer-example.json)
- [Naftiko Capability — Transfers](capabilities/transfers.yaml)

### Paystack Splits and Subaccounts API
Build marketplaces by automatically splitting a single payment between the main account and multiple subaccounts. Percentage or flat splits with configurable fee-bearers.

**Human URL:** [https://paystack.com/docs/api/split/](https://paystack.com/docs/api/split/)

- [Documentation — Split](https://paystack.com/docs/api/split/)
- [Documentation — Subaccount](https://paystack.com/docs/api/subaccount/)
- [OpenAPI](openapi/paystack-splits-subaccounts-openapi.yml)
- [JSON Schema — Split](json-schema/paystack-split-schema.json)
- [JSON Schema — Subaccount](json-schema/paystack-subaccount-schema.json)
- [JSON Structure — Split](json-structure/paystack-split-structure.json)
- [Example — Create Split](examples/paystack-create-split-example.json)
- [Naftiko Capability — Splits and Subaccounts](capabilities/splits-subaccounts.yaml)

### Paystack Dedicated Virtual Accounts API
Provision dedicated NUBAN virtual bank accounts for individual customers so they can pay by bank transfer with automatic reconciliation.

**Human URL:** [https://paystack.com/docs/api/dedicated-virtual-account/](https://paystack.com/docs/api/dedicated-virtual-account/)

- [OpenAPI](openapi/paystack-dedicated-virtual-accounts-openapi.yml)
- [Example — Create Dedicated Account](examples/paystack-create-dedicated-account-example.json)
- [Naftiko Capability — Dedicated Virtual Accounts](capabilities/dedicated-virtual-accounts.yaml)

### Paystack Products and Payment Pages API
Manage products in your Paystack inventory and assemble them into Paystack-hosted Payment Pages so you can collect payments without operating your own checkout.

**Human URL:** [https://paystack.com/docs/api/products/](https://paystack.com/docs/api/products/)

- [OpenAPI](openapi/paystack-products-pages-openapi.yml)
- [Naftiko Capability — Products and Pages](capabilities/products-pages.yaml)

### Paystack Payment Requests API
Issue invoice-style payment requests by email with verification, notification, finalization, and archival flows.

**Human URL:** [https://paystack.com/docs/api/payment-request/](https://paystack.com/docs/api/payment-request/)

- [OpenAPI](openapi/paystack-payment-requests-openapi.yml)
- [Naftiko Capability — Payment Requests](capabilities/payment-requests.yaml)

### Paystack Refunds and Disputes API
Process partial and full refunds and respond to cardholder disputes — including evidence upload via signed URL, resolution workflows, and exports.

**Human URL:** [https://paystack.com/docs/api/refund/](https://paystack.com/docs/api/refund/)

- [OpenAPI](openapi/paystack-refunds-disputes-openapi.yml)
- [JSON Schema — Refund](json-schema/paystack-refund-schema.json)
- [JSON Schema — Dispute](json-schema/paystack-dispute-schema.json)
- [Naftiko Capability — Refunds and Disputes](capabilities/refunds-disputes.yaml)

### Paystack Settlements API
Fetch settlement records and the underlying transactions that comprise each payout to your bank account.

**Human URL:** [https://paystack.com/docs/api/settlement/](https://paystack.com/docs/api/settlement/)

- [OpenAPI](openapi/paystack-settlements-openapi.yml)
- [Naftiko Capability — Settlements](capabilities/settlements.yaml)

### Paystack Verification API
Identity, BVN, bank account, card BIN, country, bank, and address-verification lookups used to validate customers, beneficiary accounts, and cards before transacting.

**Human URL:** [https://paystack.com/docs/api/verification/](https://paystack.com/docs/api/verification/)

- [OpenAPI](openapi/paystack-verification-openapi.yml)
- [Naftiko Capability — Verification](capabilities/verification.yaml)

### Paystack Balance API
Fetch your Paystack balance per currency and read the balance ledger for treasury operations and reconciliation.

**Human URL:** [https://paystack.com/docs/api/balance/](https://paystack.com/docs/api/balance/)

- [OpenAPI](openapi/paystack-balance-openapi.yml)
- [Naftiko Capability — Balance](capabilities/balance.yaml)

### Paystack Integration Settings API
Read and update integration-wide settings such as the payment session timeout for hosted checkout.

**Human URL:** [https://paystack.com/docs/api/integration/](https://paystack.com/docs/api/integration/)

- [OpenAPI](openapi/paystack-integration-openapi.yml)
- [Naftiko Capability — Integration Settings](capabilities/integration.yaml)

## Common Properties

- [Portal](https://paystack.com/)
- [Documentation](https://paystack.com/docs/)
- [API Reference](https://paystack.com/docs/api/)
- [Original Paystack OpenAPI specification](https://github.com/PaystackHQ/openapi)
- [Getting Started](https://paystack.com/docs/payments/accept-payments/)
- [Sign Up](https://dashboard.paystack.com/#/signup)
- [Dashboard](https://dashboard.paystack.com/)
- [Authentication](https://paystack.com/docs/api/#authentication)
- [API Keys](https://dashboard.paystack.com/#/settings/developers)
- [Webhooks](https://paystack.com/docs/payments/webhooks/)
- [Test Cards](https://paystack.com/docs/payments/test-payments/)
- [Errors](https://paystack.com/docs/api/errors/)
- [Change Log](https://paystack.com/docs/changelog/api/)
- [Blog](https://paystack.com/blog/)
- [Engineering Blog](https://medium.com/paystack-engineering)
- [Status Page](https://status.paystack.com/)
- [Support](https://support.paystack.com/)
- [Pricing — Nigeria](https://paystack.com/ng/pricing)
- [Pricing — Ghana](https://paystack.com/gh/pricing)
- [Pricing — South Africa](https://paystack.com/za/pricing)
- [Pricing — Kenya](https://paystack.com/ke/pricing)
- [Pricing — Côte d'Ivoire](https://paystack.com/ci/pricing)
- [Pricing — Egypt](https://paystack.com/eg/pricing)
- [Terms of Service](https://paystack.com/terms)
- [Privacy Policy](https://paystack.com/privacy)
- [Security and Compliance](https://paystack.com/security)
- [GitHub Organization](https://github.com/PaystackHQ)
- [Spectral Rules](rules/paystack-rules.yml)
- [Vocabulary](vocabulary/paystack-vocabulary.yml)
- [JSON-LD Context](json-ld/paystack-context.jsonld)
- [Plans and Pricing](plans/paystack-plans-pricing.yml)
- [Rate Limits](rate-limits/paystack-rate-limits.yml)
- [FinOps](finops/paystack-finops.yml)

## SDKs and Plugins

- [Paystack PHP Library](https://github.com/PaystackHQ/paystack-php)
- [Paystack Android SDK](https://github.com/PaystackHQ/paystack-android)
- [Paystack iOS SDK (Objective-C)](https://github.com/PaystackHQ/paystack-ios)
- [Paystack iOS SDK (Swift)](https://github.com/PaystackHQ/paystack-sdk-ios)
- [Omnipay Paystack Driver](https://github.com/PaystackHQ/omnipay-paystack)
- [WooCommerce Plugin](https://github.com/PaystackHQ/plugin-woocommerce)
- [Magento 2 Plugin](https://github.com/PaystackHQ/plugin-magento-2)
- [PrestaShop 1.7 Plugin](https://github.com/PaystackHQ/plugin-prestashop-1.7)
- [OpenCart Plugin](https://github.com/PaystackHQ/plugin-opencart)
- [WHMCS Plugin](https://github.com/PaystackHQ/plugin-whmcs)
- [Moodle Enrolment Plugin](https://github.com/PaystackHQ/moodle-enrol_paystack)
- [Odoo 14 Plugin](https://github.com/PaystackHQ/plugin-odoo)
- [Paystack JS Sample Code](https://github.com/PaystackHQ/PaystackJS-Sample-code)
- [Sample Charge Card Backend](https://github.com/PaystackHQ/sample-charge-card-backend)

## Maintainers

- **Kin Lane** — [API Evangelist](https://apievangelist.com) — info@apievangelist.com — [@apievangelist](https://x.com/apievangelist)
