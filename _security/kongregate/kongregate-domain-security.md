---
api_specs:
- filename: kongregate-server-api-openapi-original.json
  format: json
  label: Kongregate Server-Side API
  slug: kongregate-server-side-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kongregate/refs/heads/main/openapi/kongregate-server-api-openapi-original.json
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "comodoca.com"
  dmarc: false
  dnssec: true
  domain: kongregate.com
  spf: true
hosts:
- cert_expires: Dec 18 15:39:08 2026 GMT
  host: www.kongregate.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 18 15:39:08 2026 GMT
  host: api.kongregate.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Kongregate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kongregate, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Kongregate
provider_slug: kongregate
slug: kongregate-domain-security
source_filename: kongregate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kongregate.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 18 15:39:08 2026 GMT\n  hsts: false\n- host: api.kongregate.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 18 15:39:08 2026 GMT\n  hsts: null\ndomains:\n- domain: kongregate.com\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kongregate/refs/heads/main/security/kongregate-domain-security.yml
summary_line: TLSv1.2 · DNSSEC
tags:
- Company
- Gaming
- Games
- Game Development
- Browser Games
- Virtual Goods
- Microtransactions
- Leaderboards
- Player Identity
- Unity
- Developer Platform
---
