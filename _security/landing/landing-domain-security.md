---
api_specs:
- filename: landing-public-openapi.json
  format: json
  label: Landing Public API
  slug: public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landing/refs/heads/main/openapi/landing-public-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hellolanding.com
  spf: true
hosts:
- cert_expires: Sep  3 16:18:21 2026 GMT
  host: www.hellolanding.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Landing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Landing, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Landing
provider_slug: landing
slug: landing-domain-security
source_filename: landing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hellolanding.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 16:18:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hellolanding.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/landing/refs/heads/main/security/landing-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Proptech
- Real Estate
- Rentals
- Furnished Apartments
- Corporate Housing
- Travel
- Agent Native
- MCP
- Search
---
