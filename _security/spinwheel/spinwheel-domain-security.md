---
api_specs:
- filename: spinwheel-openapi.yml
  format: yaml
  label: Spinwheel Credit Data API
  slug: credit-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spinwheel/refs/heads/main/openapi/spinwheel-openapi.yml
- filename: spinwheel-openapi.yml
  format: yaml
  label: Spinwheel Liabilities & Debt API
  slug: liabilities-debt
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spinwheel/refs/heads/main/openapi/spinwheel-openapi.yml
- filename: spinwheel-openapi.yml
  format: yaml
  label: Spinwheel Payments API
  slug: payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spinwheel/refs/heads/main/openapi/spinwheel-openapi.yml
- filename: spinwheel-openapi.yml
  format: yaml
  label: Spinwheel Users & Modules API
  slug: users-modules
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spinwheel/refs/heads/main/openapi/spinwheel-openapi.yml
- filename: spinwheel-openapi.yml
  format: yaml
  label: Spinwheel Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spinwheel/refs/heads/main/openapi/spinwheel-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: spinwheel.io
  spf: true
hosts:
- cert_expires: Sep 16 22:11:22 2026 GMT
  host: www.spinwheel.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 18:32:29 2026 GMT
  host: docs.spinwheel.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 23:59:59 2026 GMT
  host: api.spinwheel.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spinwheel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spinwheel, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Spinwheel
provider_slug: spinwheel
slug: spinwheel-domain-security
source_filename: spinwheel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.spinwheel.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 22:11:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.spinwheel.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 18:32:29 2026 GMT\n  hsts: null\n- host: api.spinwheel.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: spinwheel.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spinwheel/refs/heads/main/security/spinwheel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fintech
- Credit Data
- Debt
- Liabilities
- Payments
- Embedded Finance
---
