---
api_specs:
- filename: dun-and-bradstreet-authentication-api-openapi.yml
  format: yaml
  label: Dun & Bradstreet Authentication API
  slug: dun-and-bradstreet-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dun-and-bradstreet/refs/heads/main/openapi/dun-and-bradstreet-authentication-api-openapi.yml
- filename: dun-and-bradstreet-data-file-api-openapi.yml
  format: yaml
  label: Dun & Bradstreet Data File API
  slug: dun-and-bradstreet-data-file-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dun-and-bradstreet/refs/heads/main/openapi/dun-and-bradstreet-data-file-api-openapi.yml
- filename: dun-and-bradstreet-enrich-api-openapi.yml
  format: yaml
  label: Dun & Bradstreet Enrich API
  slug: dun-and-bradstreet-enrich-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dun-and-bradstreet/refs/heads/main/openapi/dun-and-bradstreet-enrich-api-openapi.yml
- filename: dun-and-bradstreet-identity-resolution-api-openapi.yml
  format: yaml
  label: Dun & Bradstreet Identity Resolution API
  slug: dun-and-bradstreet-identity-resolution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dun-and-bradstreet/refs/heads/main/openapi/dun-and-bradstreet-identity-resolution-api-openapi.yml
- filename: dun-and-bradstreet-monitoring-api-openapi.yml
  format: yaml
  label: Dun & Bradstreet Monitoring API
  slug: dun-and-bradstreet-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dun-and-bradstreet/refs/heads/main/openapi/dun-and-bradstreet-monitoring-api-openapi.yml
- filename: dun-and-bradstreet-multi-process-api-openapi.yml
  format: yaml
  label: Dun & Bradstreet Multi-Process API
  slug: dun-and-bradstreet-multi-process-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dun-and-bradstreet/refs/heads/main/openapi/dun-and-bradstreet-multi-process-api-openapi.yml
- filename: dun-and-bradstreet-research-api-openapi.yml
  format: yaml
  label: Dun & Bradstreet Research API
  slug: dun-and-bradstreet-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dun-and-bradstreet/refs/heads/main/openapi/dun-and-bradstreet-research-api-openapi.yml
- filename: dun-and-bradstreet-search-api-openapi.yml
  format: yaml
  label: Dun & Bradstreet Search API
  slug: dun-and-bradstreet-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dun-and-bradstreet/refs/heads/main/openapi/dun-and-bradstreet-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dnb.com
  spf: true
hosts:
- cert_expires: Aug 21 17:14:25 2026 GMT
  host: www.dnb.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 17:41:43 2026 GMT
  host: directplus.documentation.dnb.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: plus.dnb.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dun And Bradstreet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dun & Bradstreet, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Dun & Bradstreet
provider_slug: dun-and-bradstreet
slug: dun-and-bradstreet-domain-security
source_filename: dun-and-bradstreet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dnb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 17:14:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: directplus.documentation.dnb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 17:41:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: plus.dnb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: dnb.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dun-and-bradstreet/refs/heads/main/security/dun-and-bradstreet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Business Data
- Company Data
- D-U-N-S Number
- Credit
- Risk
- Master Data
- Data Enrichment
- Identity Resolution
- Compliance
- Supply Chain
- Sales Intelligence
- Monitoring
---
