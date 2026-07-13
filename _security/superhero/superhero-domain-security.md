---
api_specs:
- filename: openapi.yml
  format: yaml
  label: Superhero API
  slug: superhero-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superhero/refs/heads/main/openapi/openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: superheroapi.com
  spf: true
hosts:
- cert_expires: Aug 14 03:34:48 2026 GMT
  host: www.superheroapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 03:34:48 2026 GMT
  host: superheroapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Superhero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Superhero API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Superhero API
provider_slug: superhero
slug: superhero-domain-security
source_filename: superhero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.superheroapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 03:34:48 2026 GMT\n  hsts: false\n- host: superheroapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 03:34:48 2026 GMT\n  hsts: false\ndomains:\n- domain: superheroapi.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superhero/refs/heads/main/security/superhero-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Superheroes
- Comics
- Characters
- Marvel
- DC Comics
- Entertainment
- Open Data
---
