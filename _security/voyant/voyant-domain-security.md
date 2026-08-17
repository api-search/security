---
api_specs:
- filename: voyant-openapi-original.json
  format: json
  label: VoyantIO API
  slug: voyantio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voyant/refs/heads/main/openapi/voyant-openapi-original.json
- filename: voyant-gypsum-openapi.json
  format: json
  label: Gypsum Context API
  slug: gypsum-context-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voyant/refs/heads/main/openapi/voyant-gypsum-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: voyant.io
  spf: true
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: railway.app
  spf: true
hosts:
- cert_expires: Oct 18 05:34:53 2026 GMT
  host: www.voyant.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 27 02:40:54 2026 GMT
  host: voice-forge-production.up.railway.app
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Voyant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Voyant.io, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Voyant.io
provider_slug: voyant
slug: voyant-domain-security
source_filename: voyant-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.voyant.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 05:34:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: voice-forge-production.up.railway.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 02:40:54 2026 GMT\n  hsts: null\ndomains:\n- domain: voyant.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: railway.app\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voyant/refs/heads/main/security/voyant-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- artificial-intelligence
- context-management
- brand-governance
- product-marketing
- gtm-operations
- marketing-automation
- content-generation
- competitive-intelligence
- semantic-search
- rag
- mcp
- agent-native
- signals
- telemetry
---
