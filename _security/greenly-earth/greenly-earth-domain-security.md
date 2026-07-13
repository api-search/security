---
api_specs:
- filename: greenly-carbon-analytics-api-openapi.yml
  format: yaml
  label: Greenly Carbon Analytics API
  slug: greenly-carbon-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenly-earth/refs/heads/main/openapi/greenly-carbon-analytics-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: greenly.earth
  spf: true
hosts:
- cert_expires: Oct  3 06:24:51 2026 GMT
  host: greenly.earth
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 05:25:12 2026 GMT
  host: api.greenly.earth
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Greenly Earth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Greenly, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Greenly
provider_slug: greenly-earth
slug: greenly-earth-domain-security
source_filename: greenly-earth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: greenly.earth\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 06:24:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.greenly.earth\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 05:25:12 2026 GMT\n  hsts: null\ndomains:\n- domain: greenly.earth\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/greenly-earth/refs/heads/main/security/greenly-earth-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Carbon Accounting
- Carbon Footprint
- Carbon Analytics
- Greenhouse Gas
- GHG Protocol
- Scope 1
- Scope 2
- Scope 3
- Sustainability
- ESG
- Climate
- CSRD
- CBAM
- EUDR
- SBTi
- TCFD
- EcoVadis
- Bilan Carbone
- Life Cycle Assessment
- Carbon Offsets
- SMB
- Fintech
- Transaction Enrichment
---
