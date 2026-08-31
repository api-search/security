---
api_specs:
- filename: payem-ai-discovery-api-openapi.yml
  format: yaml
  label: Payem AI Discovery API
  slug: payem-ai-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payem/refs/heads/main/openapi/payem-ai-discovery-api-openapi.yml
- filename: payem-business-api-openapi.yml
  format: yaml
  label: Payem Business API
  slug: payem-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payem/refs/heads/main/openapi/payem-business-api-openapi.yml
- filename: payem-categories-api-openapi.yml
  format: yaml
  label: Payem Categories API
  slug: payem-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payem/refs/heads/main/openapi/payem-categories-api-openapi.yml
- filename: payem-faq-api-openapi.yml
  format: yaml
  label: Payem Faq API
  slug: payem-faq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payem/refs/heads/main/openapi/payem-faq-api-openapi.yml
- filename: payem-qa-api-openapi.yml
  format: yaml
  label: Payem Qa API
  slug: payem-qa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payem/refs/heads/main/openapi/payem-qa-api-openapi.yml
- filename: payem-search-api-openapi.yml
  format: yaml
  label: Payem Search API
  slug: payem-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payem/refs/heads/main/openapi/payem-search-api-openapi.yml
- filename: payem-testimonials-api-openapi.yml
  format: yaml
  label: Payem Testimonials API
  slug: payem-testimonials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payem/refs/heads/main/openapi/payem-testimonials-api-openapi.yml
certifications:
- SOC 1 Type II
- SOC 2 Type II
- GDPR
- CCPA
description: ''
kind: trust-center
layout: security
name: Payem Trust Center
name_suffix: Trust Center
overview: Payem maintains a public trust center documenting SOC 1 Type II, SOC 2 Type II, GDPR, and CCPA compliance.
provider_name: Payem
provider_slug: payem
slug: payem-trust-center
source_filename: payem-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://security.payem.co/\nurl: https://security.payem.co/\ntrust_center:\n  vendor: SafeBase\n  host: security.payem.co\n  resolves_to: payem.portals.safebase.io\n  status: 403\n  reachable: false\n  note: >-\n    PayEm operates a dedicated SafeBase trust portal - security.payem.co CNAMEs to\n    payem.portals.safebase.io, a per-tenant SafeBase hostname, so the portal genuinely\n    exists. Its contents could not be read from this run: the portal, the SafeBase tenant\n    host and the SafeBase public API all answered HTTP 403 with a Cloudflare \"Just a\n    moment...\" interstitial. A bot challenge is not a dead page; the portal is recorded as\n    present but unread.\ncertifications:\n- name: SOC 1 Type II\n  source: https://www.payem.co/legal/security-and-compliance\n  evidence: >-\n    \"PayEm is committed to providing our customers with the highest standard of financial\n    data security and has attained both SOC 1 and\
  \ SOC 2 Type 2 attestation.\"\n- name: SOC 2 Type II\n  auditor: EY\n  source: https://www.payem.co/legal/security-and-compliance\n  evidence: >-\n    \"We are annually audited by third party accounting firm EY, to meet and exceed the\n    standards of SOC 2 Type II.\"\n- name: GDPR\n  source: https://www.payem.co/legal/security-and-compliance\n- name: CCPA\n  source: https://www.payem.co/legal/security-and-compliance\ncorrections:\n- '2026-08-26: an earlier automated pass recorded ISO 27001 and PCI DSS for this provider.\n  Neither claim could be substantiated - security.payem.co returns a bot challenge, and\n  neither standard is named anywhere on PayEm''s own public security and compliance page.\n  Both were removed rather than left as unsourced assertions.'\nevidence:\n- url: https://security.payem.co/\n  status: 403\n  note: Cloudflare interstitial; DNS CNAME payem.portals.safebase.io confirms a real SafeBase tenant\n- url: https://www.payem.co/legal/security-and-compliance\n  status:\
  \ 200\n- url: https://www.payem.co/legal/soc-2\n  status: 200\n- url: https://www.payem.co/legal/soc-1-type-ii-compliant\n  status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payem/refs/heads/main/security/payem-trust-center.yml
summary_line: SOC 1 Type II, SOC 2 Type II, GDPR, CCPA
tags:
- Company
- Spend Management
- Procurement
- Accounts Payable
- Corporate Cards
- Expense Management
- Financial Operations
- Invoice Processing
- FinTech
- ERP Integration
trust_url: https://security.payem.co/
---
