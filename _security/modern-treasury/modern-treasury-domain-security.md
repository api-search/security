---
api_specs:
- filename: modern-treasury-openapi.yml
  format: yaml
  label: Modern Treasury Payments API
  slug: modern-treasury-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modern-treasury/refs/heads/main/openapi/modern-treasury-openapi.yml
- filename: modern-treasury-openapi.yml
  format: yaml
  label: Modern Treasury Ledgers API
  slug: modern-treasury-ledgers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modern-treasury/refs/heads/main/openapi/modern-treasury-openapi.yml
- filename: modern-treasury-openapi.yml
  format: yaml
  label: Modern Treasury Counterparties API
  slug: modern-treasury-counterparties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modern-treasury/refs/heads/main/openapi/modern-treasury-openapi.yml
- filename: modern-treasury-openapi.yml
  format: yaml
  label: Modern Treasury Connections & Webhooks API
  slug: modern-treasury-connections-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modern-treasury/refs/heads/main/openapi/modern-treasury-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: moderntreasury.com
  spf: true
hosts:
- cert_expires: Sep 28 14:57:23 2026 GMT
  host: www.moderntreasury.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 08:24:36 2026 GMT
  host: docs.moderntreasury.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: app.moderntreasury.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Modern Treasury Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Modern Treasury, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Modern Treasury
provider_slug: modern-treasury
slug: modern-treasury-domain-security
source_filename: modern-treasury-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.moderntreasury.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 14:57:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.moderntreasury.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 08:24:36 2026 GMT\n  hsts: null\n- host: app.moderntreasury.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: moderntreasury.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modern-treasury/refs/heads/main/security/modern-treasury-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fintech
- Payments
- ACH
- Wires
- Treasury
---
