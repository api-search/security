---
api_specs:
- filename: realtyfeed-mls-router-postman.json
  format: json
  label: MLS Router API
  slug: mls-router-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/realtyfeed/refs/heads/main/postman/realtyfeed-mls-router-postman.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: realtyfeed.com
  spf: true
hosts:
- cert_expires: Dec 10 09:43:14 2026 GMT
  host: realtyfeed.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Realtyfeed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RealtyFeed, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: RealtyFeed
provider_slug: realtyfeed
slug: realtyfeed-domain-security
source_filename: realtyfeed-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: realtyfeed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 09:43:14 2026 GMT\n  hsts: false\ndomains:\n- domain: realtyfeed.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/realtyfeed/refs/heads/main/security/realtyfeed-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Real Estate
- MLS
- RESO Web API
- OData
- IDX
- Property Data
---
