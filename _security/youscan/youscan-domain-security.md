---
api_specs:
- filename: youscan-data-import-api-openapi.yml
  format: yaml
  label: YouScan Data Import API
  slug: youscan-data-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youscan/refs/heads/main/openapi/youscan-data-import-api-openapi.yml
- filename: youscan-history-api-openapi.yml
  format: yaml
  label: YouScan History API
  slug: youscan-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youscan/refs/heads/main/openapi/youscan-history-api-openapi.yml
- filename: youscan-mentions-api-openapi.yml
  format: yaml
  label: YouScan Mentions API
  slug: youscan-mentions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youscan/refs/heads/main/openapi/youscan-mentions-api-openapi.yml
- filename: youscan-spaces-api-openapi.yml
  format: yaml
  label: YouScan Spaces API
  slug: youscan-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youscan/refs/heads/main/openapi/youscan-spaces-api-openapi.yml
- filename: youscan-statistics-api-openapi.yml
  format: yaml
  label: YouScan Statistics API
  slug: youscan-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youscan/refs/heads/main/openapi/youscan-statistics-api-openapi.yml
- filename: youscan-tags-api-openapi.yml
  format: yaml
  label: YouScan Tags API
  slug: youscan-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youscan/refs/heads/main/openapi/youscan-tags-api-openapi.yml
- filename: youscan-topics-api-openapi.yml
  format: yaml
  label: YouScan Topics API
  slug: youscan-topics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youscan/refs/heads/main/openapi/youscan-topics-api-openapi.yml
- filename: youscan-webhook-api-openapi.yml
  format: yaml
  label: YouScan Webhook API
  slug: youscan-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youscan/refs/heads/main/openapi/youscan-webhook-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: youscan.io
  spf: true
hosts:
- cert_expires: Oct 20 20:50:39 2026 GMT
  host: youscan.io
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 12:10:19 2026 GMT
  host: developers.youscan.io
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  8 20:24:01 2026 GMT
  host: api.youscan.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Youscan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for YouScan, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: YouScan
provider_slug: youscan
slug: youscan-domain-security
source_filename: youscan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: youscan.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 20:50:39 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: developers.youscan.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 12:10:19 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: api.youscan.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 20:24:01 2026 GMT\n  hsts: null\ndomains:\n- domain: youscan.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/youscan/refs/heads/main/security/youscan-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Social Media Listening
- Social Intelligence
- Consumer Insights
- Sentiment Analysis
- Media Monitoring
- Analytics
- Artificial Intelligence
---
