---
api_specs:
- filename: chaossearch-bulkexport-api-openapi.yml
  format: yaml
  label: ChaosSearch Bulkexport API
  slug: chaossearch-bulkexport-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chaossearch/refs/heads/main/openapi/chaossearch-bulkexport-api-openapi.yml
- filename: chaossearch-chaossearch-api-api-openapi.yml
  format: yaml
  label: ChaosSearch ChaosSearch API
  slug: chaossearch-chaossearch-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chaossearch/refs/heads/main/openapi/chaossearch-chaossearch-api-api-openapi.yml
- filename: chaossearch-user-api-openapi.yml
  format: yaml
  label: ChaosSearch User API
  slug: chaossearch-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chaossearch/refs/heads/main/openapi/chaossearch-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: chaossearch.io
  spf: true
hosts:
- cert_expires: Nov 17 18:15:28 2026 GMT
  host: www.chaossearch.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chaossearch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ChaosSearch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ChaosSearch
provider_slug: chaossearch
slug: chaossearch-domain-security
source_filename: chaossearch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chaossearch.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 18:15:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: chaossearch.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chaossearch/refs/heads/main/security/chaossearch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Observability
- Security
- Data Lake
- Cloud Storage
- ELK
---
