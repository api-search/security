---
api_specs:
- filename: gamesight-measurement-openapi.json
  format: json
  label: Gamesight Measurement API
  slug: gamesight-measurement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gamesight/refs/heads/main/openapi/gamesight-measurement-openapi.json
- filename: gamesight-reporting-openapi.json
  format: json
  label: Gamesight Reporting API
  slug: gamesight-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gamesight/refs/heads/main/openapi/gamesight-reporting-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gamesight.io
  spf: true
hosts:
- cert_expires: Nov 18 23:59:59 2026 GMT
  host: gamesight.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 11:33:56 2026 GMT
  host: api.ingest.marketing.gamesight.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 13:00:45 2026 GMT
  host: api.marketing.gamesight.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gamesight Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gamesight, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Gamesight
provider_slug: gamesight
slug: gamesight-domain-security
source_filename: gamesight-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gamesight.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 23:59:59 2026 GMT\n  hsts: false\n- host: api.ingest.marketing.gamesight.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 11:33:56 2026 GMT\n  hsts: null\n- host: api.marketing.gamesight.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 13:00:45 2026 GMT\n  hsts: null\ndomains:\n- domain: gamesight.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gamesight/refs/heads/main/security/gamesight-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Gaming
- Marketing
- Analytics
- Attribution
- Measurement
- Advertising
- Creators
- Game Development
---
