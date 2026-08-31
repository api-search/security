---
api_specs:
- filename: sponsorunited-api-openapi.json
  format: json
  label: SponsorUnited API
  slug: sponsorunited-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sponsorunited/refs/heads/main/openapi/sponsorunited-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sponsorunited.com
  spf: true
hosts:
- cert_expires: Nov 10 20:12:13 2026 GMT
  host: www.sponsorunited.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: api.sponsorunited.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sponsorunited Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SponsorUnited, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SponsorUnited
provider_slug: sponsorunited
slug: sponsorunited-domain-security
source_filename: sponsorunited-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sponsorunited.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 20:12:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.sponsorunited.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sponsorunited.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sponsorunited/refs/heads/main/security/sponsorunited-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Sponsorship
- Sports
- Entertainment
- Marketing
- Advertising
- Media
- Data
- Analytics
- Market Intelligence
- SaaS
- Partnerships
---
