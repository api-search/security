---
api_specs:
- filename: triple-whale-api-keys-api-openapi.yml
  format: yaml
  label: Triple Whale API Keys API
  slug: triple-whale-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triple-whale/refs/heads/main/openapi/triple-whale-api-keys-api-openapi.yml
- filename: triple-whale-compliance-api-openapi.yml
  format: yaml
  label: Triple Whale Compliance API
  slug: triple-whale-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triple-whale/refs/heads/main/openapi/triple-whale-compliance-api-openapi.yml
- filename: triple-whale-data-in-api-openapi.yml
  format: yaml
  label: Triple Whale Data In API
  slug: triple-whale-data-in-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triple-whale/refs/heads/main/openapi/triple-whale-data-in-api-openapi.yml
- filename: triple-whale-data-out-api-openapi.yml
  format: yaml
  label: Triple Whale Data Out API
  slug: triple-whale-data-out-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triple-whale/refs/heads/main/openapi/triple-whale-data-out-api-openapi.yml
- filename: triple-whale-bi-api-openapi.yml
  format: yaml
  label: Triple Whale Bi API
  slug: triple-whale-bi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triple-whale/refs/heads/main/openapi/triple-whale-bi-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: triplewhale.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.io
  spf: true
hosts:
- cert_expires: Sep 23 06:12:17 2026 GMT
  host: www.triplewhale.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 13:12:37 2026 GMT
  host: triplewhale.readme.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 17:58:54 2026 GMT
  host: api.triplewhale.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Triple Whale Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Triple Whale, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Triple Whale
provider_slug: triple-whale
slug: triple-whale-domain-security
source_filename: triple-whale-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.triplewhale.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 06:12:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: triplewhale.readme.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:12:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.triplewhale.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 17:58:54 2026 GMT\n  hsts: null\ndomains:\n- domain: triplewhale.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: readme.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/triple-whale/refs/heads/main/security/triple-whale-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- E-Commerce
- Analytics
- Attribution
- Shopify
- Pixel Tracking
- ROAS
- DTC
- Marketing
---
