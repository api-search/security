---
api_specs:
- filename: archer-daniels-midland-commodity-data-api-openapi.yml
  format: yaml
  label: Archer Daniels Midland Commodity Data API
  slug: commodity-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archer-daniels-midland/refs/heads/main/openapi/archer-daniels-midland-commodity-data-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: adm.com
  spf: true
hosts:
- cert_expires: Dec  5 23:59:59 2026 GMT
  host: www.adm.com
  hsts: true
  hsts_max_age: 5184000
  https: true
  tls_version: TLSv1.3
- host: api.adm.com
  https: false
kind: domain-security
layout: security
method: probed
name: Archer Daniels Midland Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Archer Daniels Midland, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Archer Daniels Midland
provider_slug: archer-daniels-midland
slug: archer-daniels-midland-domain-security
source_filename: archer-daniels-midland-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.adm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 5184000\n- host: api.adm.com\n  https: false\ndomains:\n- domain: adm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/archer-daniels-midland/refs/heads/main/security/archer-daniels-midland-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agriculture
- Food Processing
- Commodities
- Supply Chain
- Fortune 100
- Nutrition
---
