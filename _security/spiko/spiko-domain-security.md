---
api_specs:
- filename: spiko-public-openapi.json
  format: json
  label: Spiko Public API
  slug: spiko-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spiko/refs/heads/main/openapi/spiko-public-openapi.json
- filename: spiko-investor-openapi.json
  format: json
  label: Spiko Investor API
  slug: spiko-investor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spiko/refs/heads/main/openapi/spiko-investor-openapi.json
- filename: spiko-distributor-openapi.json
  format: json
  label: Spiko Distributor API
  slug: spiko-distributor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spiko/refs/heads/main/openapi/spiko-distributor-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: spiko.io
  spf: true
hosts:
- cert_expires: Aug 23 19:13:42 2026 GMT
  host: spiko.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 23:01:01 2026 GMT
  host: distributor-api.spiko.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 10:02:09 2026 GMT
  host: distributor-api.preprod.spiko.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spiko Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spiko, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Spiko
provider_slug: spiko
slug: spiko-domain-security
source_filename: spiko-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spiko.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 19:13:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: distributor-api.spiko.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 23:01:01 2026 GMT\n  hsts: null\n- host: distributor-api.preprod.spiko.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 10:02:09 2026 GMT\n  hsts: null\ndomains:\n- domain: spiko.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spiko/refs/heads/main/security/spiko-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Money Market Funds
- Treasury Management
- Tokenization
- Cash Management
- Payments
- Webhooks
---
