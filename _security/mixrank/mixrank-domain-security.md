---
api_specs:
- filename: mixrank-openapi.yml
  format: yaml
  label: MixRank Data API
  slug: mixrank-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixrank/refs/heads/main/openapi/mixrank-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mixrank.com
  spf: true
hosts:
- cert_expires: Sep 29 23:18:46 2026 GMT
  host: mixrank.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 23:18:33 2026 GMT
  host: api.mixrank.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mixrank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MixRank, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MixRank
provider_slug: mixrank
slug: mixrank-domain-security
source_filename: mixrank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mixrank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:18:46 2026 GMT\n  hsts: false\n- host: api.mixrank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:18:33 2026 GMT\n  hsts: null\ndomains:\n- domain: mixrank.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mixrank/refs/heads/main/security/mixrank-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Data
- Technographics
- Firmographics
- People Data
- Mobile Apps
- SDK Intelligence
- App Store
- Web Technology
- Sales Intelligence
- Data Enrichment
---
