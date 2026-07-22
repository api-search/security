---
api_specs:
- filename: startree-query-openapi.json
  format: json
  label: StarTree Cloud Query API
  slug: startree-cloud-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/startree/refs/heads/main/openapi/startree-query-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: startree.ai
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: startree.cloud
  spf: false
hosts:
- cert_expires: Oct 12 10:00:32 2026 GMT
  host: startree.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: broker.pinot.celpxu.cp.s7e.startree.cloud
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Startree Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StarTree, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: StarTree
provider_slug: startree
slug: startree-domain-security
source_filename: startree-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: startree.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 10:00:32 2026 GMT\n  hsts: false\n- host: broker.pinot.celpxu.cp.s7e.startree.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: startree.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: startree.cloud\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/startree/refs/heads/main/security/startree-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Data
- Analytics
- Real-Time Analytics
- OLAP
- Apache Pinot
- Streaming
- Database
---
