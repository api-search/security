---
api_specs:
- filename: punchh-check-in-api-openapi.yml
  format: yaml
  label: Punchh Check-In API
  slug: punchh-check-in-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-check-in-api-openapi.yml
- filename: punchh-check-ins-api-openapi.yml
  format: yaml
  label: Punchh Check-Ins API
  slug: punchh-check-ins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-check-ins-api-openapi.yml
- filename: punchh-configuration-api-openapi.yml
  format: yaml
  label: Punchh Configuration API
  slug: punchh-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-configuration-api-openapi.yml
- filename: punchh-offers-api-openapi.yml
  format: yaml
  label: Punchh Offers API
  slug: punchh-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-offers-api-openapi.yml
- filename: punchh-receipts-api-openapi.yml
  format: yaml
  label: Punchh Receipts API
  slug: punchh-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-receipts-api-openapi.yml
- filename: punchh-redemptions-api-openapi.yml
  format: yaml
  label: Punchh Redemptions API
  slug: punchh-redemptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-redemptions-api-openapi.yml
- filename: punchh-users-api-openapi.yml
  format: yaml
  label: Punchh Users API
  slug: punchh-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: punchh.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: partech.com
  spf: true
hosts:
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: punchh.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 23:18:33 2026 GMT
  host: developers.partech.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Punchh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Punchh, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Punchh
provider_slug: punchh
slug: punchh-domain-security
source_filename: punchh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: punchh.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: false\n- host: developers.partech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 23:18:33 2026 GMT\n  hsts: false\ndomains:\n- domain: punchh.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: partech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/security/punchh-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Restaurant
- Loyalty
- Marketing
- Guest Engagement
- Online Ordering
- Mobile
- Point Of Sale
- Webhooks
---
