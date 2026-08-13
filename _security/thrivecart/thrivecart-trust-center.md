---
api_specs:
- filename: thrivecart-api-openapi.yml
  format: yaml
  label: ThriveCart API
  slug: thrivecart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thrivecart/refs/heads/main/openapi/thrivecart-api-openapi.yml
certifications:
- PCI DSS
- GDPR
- CCPA
description: ''
kind: trust-center
layout: security
name: Thrivecart Trust Center
name_suffix: Trust Center
overview: ThriveCart maintains a public trust center documenting PCI DSS, GDPR, and CCPA compliance.
provider_name: ThriveCart
provider_slug: thrivecart
slug: thrivecart-trust-center
source_filename: thrivecart-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://thrivecart.com/\ntrust_center_published: false\ntrust_center_url: null\nnote: >-\n  ThriveCart does not operate a trust centre. There is no trust.thrivecart.com, no security\n  portal, and no downloadable attestation report. https://trust.thrivecart.com/ resolves to the\n  ThriveCart sign-in catch-all (HTTP 200, SPA shell), not a trust portal. What ThriveCart does\n  publish is a pair of self-asserted compliance badges on its marketing homepage and a data\n  protection section in its legal terms. No third-party audit report (SOC 2, ISO 27001) is named\n  or offered anywhere on the public site.\ncertifications:\n- name: PCI DSS\n  status: self-asserted\n  evidence: 'Homepage badge: \"PCI DSS Compliant\"; feature copy: \"Always stay compliant with taxes\n    and global compliance built in (inc. PCI-DSS & GDPR).\"'\n  source: https://thrivecart.com/\n  attestation_published: false\n- name: GDPR\n  status: self-asserted\n\
  \  evidence: 'Homepage badge: \"GDPR Compliant\". Legal terms describe ThriveCart as a \"data\n    processor\" acting on behalf of its customers as defined under the GDPR.'\n  source: https://thrivecart.com/legal/thrivecart/\n  attestation_published: false\n- name: CCPA\n  status: self-asserted\n  evidence: 'Legal terms describe ThriveCart as a \"service provider\" for the purposes of the\n    California Consumer Privacy Act.'\n  source: https://thrivecart.com/legal/thrivecart/\n  attestation_published: false\nnot_found:\n- SOC 2\n- ISO 27001\n- HIPAA\n- FedRAMP\nevidence:\n- url: https://thrivecart.com/\n  http_status: 200\n  finding: PCI DSS Compliant + GDPR Compliant badges in the hero trust row\n- url: https://thrivecart.com/legal/thrivecart/\n  http_status: 200\n  finding: GDPR data-processor and CCPA service-provider language in the terms\n- url: https://trust.thrivecart.com/\n  http_status: 200\n  finding: redirects to https://thrivecart.com/signin/ (SPA catch-all) - not a trust\
  \ centre\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thrivecart/refs/heads/main/security/thrivecart-trust-center.yml
summary_line: PCI DSS, GDPR, CCPA
tags:
- Company
- Checkout
- Shopping Cart
- Payments
- eCommerce
- Subscriptions
- Affiliate Marketing
- Learning Management
- Creator Economy
- Webhooks
trust_url: ''
---
