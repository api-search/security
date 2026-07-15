---
api_specs:
- filename: braintree-payments-openapi.yml
  format: yaml
  label: Braintree Payments API
  slug: payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintree/refs/heads/main/openapi/braintree-payments-openapi.yml
- filename: braintree-webhooks-asyncapi.yml
  format: yaml
  label: Braintree Webhooks
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintree/refs/heads/main/asyncapi/braintree-webhooks-asyncapi.yml
- filename: braintree-payments-openapi.yml
  format: yaml
  label: Braintree Vault API
  slug: vault-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintree/refs/heads/main/openapi/braintree-payments-openapi.yml
- filename: braintree-subscriptions-openapi.yml
  format: yaml
  label: Braintree Subscriptions API
  slug: subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintree/refs/heads/main/openapi/braintree-subscriptions-openapi.yml
certifications:
- PCI DSS
- Visa Global Registry of Service Providers
- Mastercard SDP
- SOC 2 Type 2
description: Braintree's security & compliance posture, captured from the Braintree PCI compliance documentation and the PayPal Trust Center. Braintree (a PayPal service) is validated as a PCI DSS Level 1 Service Provider — the most stringent level in the payments industry — and appears on Visa's Global Registry of Service Providers and Mastercard's SDP list. Braintree never stores raw magnetic-stripe, CVV, or PIN-block data; cardholder data in the Vault is encrypted with multiple keys under split-knowledge / dual-control. Merchants still complete an annual SAQ (typically SAQ A when using Hosted Fields, Drop-in, mobile SDKs, or GraphQL).
kind: trust-center
layout: security
name: Braintree Trust Center
name_suffix: Trust Center
overview: braintree maintains a public trust center documenting PCI DSS, Visa Global Registry of Service Providers, Mastercard SDP, and SOC 2 Type 2 compliance.
provider_name: braintree
provider_slug: braintree
slug: braintree-trust-center
source_filename: braintree-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-14'\nmethod: searched\nprobe: false\nsource: https://developer.paypal.com/braintree/articles/risk-and-security/compliance/pci-compliance\nurl: https://developer.paypal.com/braintree/articles/risk-and-security/compliance/overview\ndescription: >-\n  Braintree's security & compliance posture, captured from the Braintree PCI\n  compliance documentation and the PayPal Trust Center. Braintree (a PayPal\n  service) is validated as a PCI DSS Level 1 Service Provider — the most\n  stringent level in the payments industry — and appears on Visa's Global\n  Registry of Service Providers and Mastercard's SDP list. Braintree never\n  stores raw magnetic-stripe, CVV, or PIN-block data; cardholder data in the\n  Vault is encrypted with multiple keys under split-knowledge / dual-control.\n  Merchants still complete an annual SAQ (typically SAQ A when using Hosted\n  Fields, Drop-in, mobile SDKs, or GraphQL).\ncertifications:\n  - {name: PCI DSS, level: Service Provider\
  \ Level 1, note: Most stringent level; validated annually.}\n  - {name: Visa Global Registry of Service Providers, note: Listed as a compliant service provider.}\n  - {name: Mastercard SDP, note: Listed on the Site Data Protection compliant-provider list.}\n  - {name: SOC 2 Type 2, scope: PayPal/Braintree services, note: PayPal produces annual SOC reports; bridge letters updated quarterly.}\nmerchant_obligations:\n  saq: Merchants complete an annual PCI SAQ; SAQ A eligibility for Hosted Fields, Drop-in UI, mobile SDKs, and GraphQL.\n  data_handling: Braintree does not store raw magnetic-stripe, card-validation-code, or PIN-block data.\ntrust_center: https://www.paypal-trustcenter.com/\ndocs:\n  - https://developer.paypal.com/braintree/articles/risk-and-security/compliance/pci-compliance\n  - https://developer.paypal.com/braintree/articles/risk-and-security/compliance/overview\nevidence:\n  - {source: https://developer.paypal.com/braintree/articles/risk-and-security/compliance/pci-compliance,\
  \ keywords: [pci dss level 1, service provider, visa global registry, mastercard sdp, saq a]}\n  - {source: https://www.paypal-trustcenter.com/, keywords: [soc 2, trust center, compliance]}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/braintree/refs/heads/main/security/braintree-trust-center.yml
summary_line: PCI DSS, Visa Global Registry of Service Providers, Mastercard SDP, SOC 2 Type 2
tags: []
trust_url: https://developer.paypal.com/braintree/articles/risk-and-security/compliance/overview
---
