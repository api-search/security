---
api_specs:
- filename: api-league-openapi.json
  format: json
  label: API League Platform
  slug: api-league-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-league/refs/heads/main/openapi/_original/api-league-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apileague.com
  spf: true
hosts:
- cert_expires: Nov 14 20:02:43 2026 GMT
  host: apileague.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 29 09:23:25 2026 GMT
  host: api.apileague.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Api League Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for API League, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: API League
provider_slug: api-league
slug: api-league-domain-security
source_filename: api-league-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apileague.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 20:02:43 2026 GMT\n  hsts: false\n- host: api.apileague.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 09:23:25 2026 GMT\n  hsts: null\ndomains:\n- domain: apileague.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api-league/refs/heads/main/security/api-league-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- API Marketplace
- Books
- Developer Tools
- Food
- Games
- Humor
- Media
- News
- OpenAPI
- SDK
- Text Processing
- Web Scraping
---
