---
api_specs:
- filename: mintlify-openapi.yml
  format: yaml
  label: Mintlify
  slug: mintlify
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mintlify/refs/heads/main/openapi/mintlify-openapi.yml
- filename: mintlify-openapi.yml
  format: yaml
  label: Mintlify Update API
  slug: update-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mintlify/refs/heads/main/openapi/mintlify-openapi.yml
- filename: mintlify-openapi.yml
  format: yaml
  label: Mintlify Agent API
  slug: agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mintlify/refs/heads/main/openapi/mintlify-openapi.yml
- filename: mintlify-openapi.yml
  format: yaml
  label: Mintlify Assistant API
  slug: assistant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mintlify/refs/heads/main/openapi/mintlify-openapi.yml
- filename: mintlify-openapi.yml
  format: yaml
  label: Mintlify Analytics API
  slug: analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mintlify/refs/heads/main/openapi/mintlify-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mintlify.com
  spf: true
hosts:
- cert_expires: Sep 26 19:20:43 2026 GMT
  host: www.mintlify.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 14:47:25 2026 GMT
  host: api.mintlify.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mintlify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mintlify, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mintlify
provider_slug: mintlify
slug: mintlify-domain-security
source_filename: mintlify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mintlify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 19:20:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.mintlify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 14:47:25 2026 GMT\n  hsts: null\ndomains:\n- domain: mintlify.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mintlify/refs/heads/main/security/mintlify-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Documentation
---
