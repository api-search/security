---
api_specs:
- filename: zendit-api.yml
  format: yaml
  label: Zendit API
  slug: zendit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zendit/refs/heads/main/openapi/zendit-api.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zendit.io
  spf: true
hosts:
- cert_expires: Sep 29 05:23:06 2026 GMT
  host: zendit.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: api.zendit.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zendit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zendit, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Zendit
provider_slug: zendit
slug: zendit-domain-security
source_filename: zendit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zendit.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 05:23:06 2026 GMT\n  hsts: false\n- host: api.zendit.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: zendit.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zendit/refs/heads/main/security/zendit-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- eSIM
- Gift Cards
- Mobile Top-Up
- Payments
- Prepaid
---
