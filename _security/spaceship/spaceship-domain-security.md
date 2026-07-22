---
api_specs:
- filename: spaceship-openapi-original.json
  format: json
  label: Spaceship API
  slug: spaceship-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spaceship/refs/heads/main/openapi/spaceship-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: spaceshipapp.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: spaceship.dev
  spf: false
hosts:
- cert_expires: Sep 19 19:16:47 2026 GMT
  host: spaceshipapp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 21:11:24 2026 GMT
  host: spaceship.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spaceship Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spaceship, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Spaceship
provider_slug: spaceship
slug: spaceship-domain-security
source_filename: spaceship-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spaceshipapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 19:16:47 2026 GMT\n  hsts: false\n- host: spaceship.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 21:11:24 2026 GMT\n  hsts: null\ndomains:\n- domain: spaceshipapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: spaceship.dev\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spaceship/refs/heads/main/security/spaceship-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Domains
- Domain Registrar
- DNS
- Domain Marketplace
- Nameservers
- WHOIS
- Developer Tools
- API
---
