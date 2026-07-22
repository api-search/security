---
api_specs:
- filename: padlet-openapi.yml
  format: yaml
  label: Padlet API
  slug: padlet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/padlet/refs/heads/main/openapi/padlet-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: padlet.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: padlet.dev
  spf: true
hosts:
- cert_expires: Oct 12 08:29:50 2026 GMT
  host: padlet.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 09:02:36 2026 GMT
  host: api.padlet.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Padlet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Padlet, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Padlet
provider_slug: padlet
slug: padlet-domain-security
source_filename: padlet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: padlet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 08:29:50 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.padlet.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 09:02:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: padlet.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: padlet.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/padlet/refs/heads/main/security/padlet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Collaboration
- Education
- Visual Collaboration
- Content
- Boards
- Productivity
- JSON:API
- MCP
- EdTech
---
