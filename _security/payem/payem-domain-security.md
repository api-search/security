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
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: payem.co
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: llm-discovery-api.com
  spf: true
hosts:
- cert_expires: Sep 30 15:44:40 2026 GMT
  host: www.payem.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 23:40:58 2026 GMT
  host: api.llm-discovery-api.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Payem Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Payem, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Payem
provider_slug: payem
slug: payem-domain-security
source_filename: payem-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.payem.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 15:44:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.llm-discovery-api.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 23:40:58 2026 GMT\n  hsts: null\ndomains:\n- domain: payem.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: llm-discovery-api.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payem/refs/heads/main/security/payem-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
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
---
