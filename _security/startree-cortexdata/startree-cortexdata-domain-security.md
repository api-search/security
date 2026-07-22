---
api_specs:
- filename: startree-cortexdata-query-openapi.json
  format: json
  label: StarTree Cloud Query API
  slug: startree-cloud-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/startree-cortexdata/refs/heads/main/openapi/startree-cortexdata-query-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: startree.ai
  spf: true
hosts:
- cert_expires: Oct 12 02:02:52 2026 GMT
  host: www.startree.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Startree Cortexdata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StarTree (Cortexdata), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: StarTree (Cortexdata)
provider_slug: startree-cortexdata
slug: startree-cortexdata-domain-security
source_filename: startree-cortexdata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.startree.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 02:02:52 2026 GMT\n  hsts: false\ndomains:\n- domain: startree.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/startree-cortexdata/refs/heads/main/security/startree-cortexdata-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ai Infrastructure
- Real-Time Analytics
- Apache Pinot
- OLAP
- Analytics
- Streaming Data
- Database
---
