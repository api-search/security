---
api_specs:
- filename: disney-openapi.yml
  format: yaml
  label: Disney API (REST)
  slug: disney-api-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/disney/refs/heads/main/openapi/disney-openapi.yml
description: ''
domains:
- caa:
  - manucastrillonm.github.io.
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "sectigo.com"
  dmarc: false
  dnssec: true
  domain: disneyapi.dev
  spf: true
hosts:
- cert_expires: Sep 20 11:24:51 2026 GMT
  host: disneyapi.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 23:24:30 2026 GMT
  host: api.disneyapi.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Disney Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Disney API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Disney API
provider_slug: disney
slug: disney-domain-security
source_filename: disney-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: disneyapi.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 11:24:51 2026 GMT\n  hsts: false\n- host: api.disneyapi.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:24:30 2026 GMT\n  hsts: false\ndomains:\n- domain: disneyapi.dev\n  dnssec: true\n  caa:\n  - manucastrillonm.github.io.\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"sectigo.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/disney/refs/heads/main/security/disney-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Entertainment
- Characters
- Disney
- Open Source
- Fan API
- REST
- GraphQL
---
