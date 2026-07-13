---
api_specs:
- filename: walt-disney-disney-api-openapi.yml
  format: yaml
  label: Disney Characters API
  slug: disney-characters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/walt-disney/refs/heads/main/openapi/walt-disney-disney-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: disney.com
  spf: true
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
- cert_expires: Sep 21 07:22:05 2026 GMT
  host: www.disney.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 11:24:51 2026 GMT
  host: disneyapi.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: developer.disney.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Walt Disney Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Walt Disney, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Walt Disney
provider_slug: walt-disney
slug: walt-disney-domain-security
source_filename: walt-disney-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.disney.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 07:22:05 2026 GMT\n  hsts: null\n- host: disneyapi.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 11:24:51 2026 GMT\n  hsts: false\n- host: developer.disney.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: disney.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: disneyapi.dev\n  dnssec: true\n  caa:\n  - manucastrillonm.github.io.\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"sectigo.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/walt-disney/refs/heads/main/security/walt-disney-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Fortune 100
- Entertainment
- Media
- Streaming
- Parks
- Content
---
