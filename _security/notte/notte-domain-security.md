---
api_specs:
- filename: notte-openapi.yml
  format: yaml
  label: Notte Sessions API
  slug: sessions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notte/refs/heads/main/openapi/notte-openapi.yml
- filename: notte-openapi.yml
  format: yaml
  label: Notte Agents API
  slug: agents
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notte/refs/heads/main/openapi/notte-openapi.yml
- filename: notte-openapi.yml
  format: yaml
  label: Notte Page Observe / Step / Scrape API
  slug: page
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notte/refs/heads/main/openapi/notte-openapi.yml
- filename: notte-openapi.yml
  format: yaml
  label: Notte Scraping API
  slug: scrape
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notte/refs/heads/main/openapi/notte-openapi.yml
- filename: notte-openapi.yml
  format: yaml
  label: Notte Personas and Vaults API
  slug: personas-vaults
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notte/refs/heads/main/openapi/notte-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: notte.cc
  spf: true
hosts:
- cert_expires: Sep 21 07:50:16 2026 GMT
  host: notte.cc
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 02:56:34 2026 GMT
  host: docs.notte.cc
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 12:30:11 2026 GMT
  host: api.notte.cc
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Notte Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Notte, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Notte
provider_slug: notte
slug: notte-domain-security
source_filename: notte-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: notte.cc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 07:50:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.notte.cc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 02:56:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.notte.cc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 12:30:11 2026 GMT\n  hsts: null\ndomains:\n- domain: notte.cc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/notte/refs/heads/main/security/notte-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Web Agents
- Browser Automation
- Sessions
- Scraping
---
