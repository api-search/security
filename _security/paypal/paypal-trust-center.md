---
api_specs:
- filename: paypal-billing-subscriptions-openapi-original.yml
  format: yaml
  label: PayPal Billing Subscriptions API
  slug: paypal-billing-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-billing-subscriptions-openapi-original.yml
- filename: paypal-catalog-products-openapi-original.yml
  format: yaml
  label: PayPal Catalog Products API
  slug: paypal-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-catalog-products-openapi-original.yml
- filename: paypal-checkout-orders-openapi-original.yml
  format: yaml
  label: PayPal Orders API
  slug: paypal-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-checkout-orders-openapi-original.yml
- filename: paypal-customer-disputes-openapi-original.yml
  format: yaml
  label: PayPal Customer Disputes API
  slug: paypal-disputes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-customer-disputes-openapi-original.yml
- filename: paypal-customer-partner-referrals-openapi-original.yml
  format: yaml
  label: PayPal Partner Referrals API
  slug: paypal-partner-referrals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-customer-partner-referrals-openapi-original.yml
- filename: paypal-invoicing-openapi-original.yml
  format: yaml
  label: PayPal Invoicing API
  slug: paypal-invoicing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-invoicing-openapi-original.yml
- filename: paypal-notification-webhooks-openapi-original.yml
  format: yaml
  label: PayPal Notification Webhooks API
  slug: paypal-notification-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-notification-webhooks-openapi-original.yml
- filename: paypal-payment-experience-openapi-original.yml
  format: yaml
  label: PayPal Payment Experience API
  slug: paypal-payment-experience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-payment-experience-openapi-original.yml
- filename: paypal-payments-openapi-original.yml
  format: yaml
  label: PayPal Payments API
  slug: paypal-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-payments-openapi-original.yml
- filename: paypal-payouts-openapi-original.yml
  format: yaml
  label: PayPal Payouts API
  slug: paypal-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-payouts-openapi-original.yml
- filename: paypal-reporting-transactions-openapi-original.yml
  format: yaml
  label: PayPal Transaction Search (Reporting) API
  slug: paypal-reporting-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-reporting-transactions-openapi-original.yml
- filename: paypal-shipping-tracking-openapi-original.yml
  format: yaml
  label: PayPal Shipping Tracking API
  slug: paypal-shipping-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-shipping-tracking-openapi-original.yml
- filename: paypal-vault-payment-tokens-openapi-original.yml
  format: yaml
  label: PayPal Vault Payment Tokens API
  slug: paypal-payment-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-vault-payment-tokens-openapi-original.yml
certifications:
- PCI DSS
- PCI P2PE
- ISO/IEC 27001
- SOC 1
- SOC 2 Type II
description: PayPal's security & compliance posture, captured from the PayPal Trust Center (paypal-trustcenter.com, powered by SafeBase). PayPal operates as a PCI DSS Level 1 payment provider and maintains ISO/IEC 27001, PCI P2PE, and SOC 1 / SOC 2 reporting; full reports and bridge letters are gated behind Trust Center verification. This is the searched, human-verified fill (the automated probe does not clear the trust.<domain> keyword threshold since PayPal's trust center is on a distinct SafeBase-hosted domain).
kind: trust-center
layout: security
name: Paypal Trust Center
name_suffix: Trust Center
overview: PayPal maintains a public trust center documenting PCI DSS, PCI P2PE, ISO/IEC 27001, SOC 1, and SOC 2 Type II compliance.
provider_name: PayPal
provider_slug: paypal
slug: paypal-trust-center
source_filename: paypal-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-14'\nmethod: searched\nprobe: false\nsource: https://www.paypal-trustcenter.com/\nurl: https://www.paypal-trustcenter.com/\ndescription: >-\n  PayPal's security & compliance posture, captured from the PayPal Trust Center\n  (paypal-trustcenter.com, powered by SafeBase). PayPal operates as a PCI DSS\n  Level 1 payment provider and maintains ISO/IEC 27001, PCI P2PE, and SOC 1 /\n  SOC 2 reporting; full reports and bridge letters are gated behind Trust Center\n  verification. This is the searched, human-verified fill (the automated probe\n  does not clear the trust.<domain> keyword threshold since PayPal's trust\n  center is on a distinct SafeBase-hosted domain).\ncertifications:\n  - {name: PCI DSS, level: Level 1 service provider, note: Highest level for payment processors; Attestation of Compliance available.}\n  - {name: PCI P2PE, scope: Point-to-point encryption for in-person card acceptance.}\n  - {name: ISO/IEC 27001, note: Information Security Management\
  \ System (ISMS) certification.}\n  - {name: SOC 1, availability: gated, note: Report on controls over financial reporting.}\n  - {name: SOC 2 Type II, availability: gated, cadence: annual, note: Report + quarterly bridge letters; also covers Simility (fraud prevention).}\nreport_access:\n  portal: https://www.paypal-trustcenter.com/\n  gating: Reports and bridge letters are downloadable after Trust Center verification (SafeBase NDA/verification flow).\n  cadence: Compliance documentation and bridge letters updated quarterly.\nnotes: >-\n  Venmo (a PayPal service) received PCI DSS certification against the v4.0.1\n  standard per a recent Trust Center update.\nevidence:\n  - {source: https://www.paypal-trustcenter.com/, keywords: [pci dss, pci p2pe, iso/iec 27001, soc 1, soc 2, trust center]}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/security/paypal-trust-center.yml
summary_line: PCI DSS, PCI P2PE, ISO/IEC 27001, SOC 1, SOC 2 Type II
tags:
- Billing
- Commerce
- Disputes
- Invoices
- Orders
- Payments
- Payouts
- Subscriptions
- Tokens
- Webhooks
trust_url: https://www.paypal-trustcenter.com/
---
