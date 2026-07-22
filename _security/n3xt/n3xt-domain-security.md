---
api_specs:
- filename: n3xt-openapi-original.json
  format: json
  label: N3XT API
  slug: n3xt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n3xt/refs/heads/main/openapi/n3xt-openapi-original.json
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:infosec@n3xt.io"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: n3xt.io
  spf: true
hosts:
- cert_expires: Aug 27 00:35:25 2026 GMT
  host: n3xt.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 21:10:37 2026 GMT
  host: openapi.n3xt.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: N3Xt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for N3XT, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: N3XT
provider_slug: n3xt
slug: n3xt-domain-security
source_filename: n3xt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: n3xt.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 00:35:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: openapi.n3xt.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 21:10:37 2026 GMT\n  hsts: null\ndomains:\n- domain: n3xt.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:infosec@n3xt.io\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/n3xt/refs/heads/main/security/n3xt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto
- Banking
- Payments
- Stablecoin
- Fintech
- Blockchain
- API
- MCP
---
