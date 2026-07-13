---
api_specs:
- filename: fonoa-validate-openapi.yml
  format: yaml
  label: Fonoa Validate API
  slug: validate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fonoa/refs/heads/main/openapi/fonoa-validate-openapi.yml
- filename: fonoa-tax-engine-openapi.yml
  format: yaml
  label: Fonoa Tax Engine API
  slug: tax-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fonoa/refs/heads/main/openapi/fonoa-tax-engine-openapi.yml
- filename: fonoa-e-invoicing-openapi.yml
  format: yaml
  label: Fonoa E-Invoicing API
  slug: e-invoicing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fonoa/refs/heads/main/openapi/fonoa-e-invoicing-openapi.yml
- filename: fonoa-onboarding-openapi.yml
  format: yaml
  label: Fonoa Onboarding API
  slug: onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fonoa/refs/heads/main/openapi/fonoa-onboarding-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: fonoa.com
  spf: true
hosts:
- cert_expires: Sep 29 01:42:26 2026 GMT
  host: www.fonoa.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 20:48:59 2026 GMT
  host: docs.fonoa.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 05:46:58 2026 GMT
  host: api.fonoa.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fonoa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fonoa, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Fonoa
provider_slug: fonoa
slug: fonoa-domain-security
source_filename: fonoa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fonoa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 01:42:26 2026 GMT\n  hsts: false\n- host: docs.fonoa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 20:48:59 2026 GMT\n  hsts: null\n- host: api.fonoa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 05:46:58 2026 GMT\n  hsts: null\ndomains:\n- domain: fonoa.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fonoa/refs/heads/main/security/fonoa-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Tax
- VAT
- GST
- E-Invoicing
- Tax Automation
- Tax Compliance
- Tax Calculation
- Tax ID Validation
- Invoice Generation
- Global Tax
- Indirect Tax
- FinTech
---
