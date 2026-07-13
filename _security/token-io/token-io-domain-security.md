---
api_specs:
- filename: token-io-openapi.yml
  format: yaml
  label: Token.io Open Banking API
  slug: token-io-open-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/token-io/refs/heads/main/openapi/token-io-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "sectigo.com"
  - 0 iodef "mailto:security@token.io"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: token.io
  spf: true
hosts:
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: token.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 00:33:34 2026 GMT
  host: docs.token.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: api.token.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Token Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for token-io, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: token-io
provider_slug: token-io
slug: token-io-domain-security
source_filename: token-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: token.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: null\n- host: docs.token.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 00:33:34 2026 GMT\n  hsts: false\n- host: api.token.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: token.io\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 iodef \"mailto:security@token.io\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/token-io/refs/heads/main/security/token-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags: []
---
