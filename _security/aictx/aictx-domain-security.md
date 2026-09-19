---
api_specs:
- filename: aictx-awards-api-openapi.yml
  format: yaml
  label: aiCTX (now SynSense) Awards API
  slug: aictx-awards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aictx/refs/heads/main/openapi/aictx-awards-api-openapi.yml
- filename: aictx-careers-api-openapi.yml
  format: yaml
  label: aiCTX (now SynSense) Careers API
  slug: aictx-careers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aictx/refs/heads/main/openapi/aictx-careers-api-openapi.yml
- filename: aictx-company-api-openapi.yml
  format: yaml
  label: aiCTX (now SynSense) Company API
  slug: aictx-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aictx/refs/heads/main/openapi/aictx-company-api-openapi.yml
- filename: aictx-content-api-openapi.yml
  format: yaml
  label: aiCTX (now SynSense) Content API
  slug: aictx-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aictx/refs/heads/main/openapi/aictx-content-api-openapi.yml
- filename: aictx-discovery-api-openapi.yml
  format: yaml
  label: aiCTX (now SynSense) Discovery API
  slug: aictx-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aictx/refs/heads/main/openapi/aictx-discovery-api-openapi.yml
- filename: aictx-news-api-openapi.yml
  format: yaml
  label: aiCTX (now SynSense) News API
  slug: aictx-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aictx/refs/heads/main/openapi/aictx-news-api-openapi.yml
- filename: aictx-partners-api-openapi.yml
  format: yaml
  label: aiCTX (now SynSense) Partners API
  slug: aictx-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aictx/refs/heads/main/openapi/aictx-partners-api-openapi.yml
- filename: aictx-products-api-openapi.yml
  format: yaml
  label: aiCTX (now SynSense) Products API
  slug: aictx-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aictx/refs/heads/main/openapi/aictx-products-api-openapi.yml
- filename: aictx-taxonomy-api-openapi.yml
  format: yaml
  label: aiCTX (now SynSense) Taxonomy API
  slug: aictx-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aictx/refs/heads/main/openapi/aictx-taxonomy-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: synsense.ai
  spf: true
hosts:
- cert_expires: Nov 17 06:43:24 2026 GMT
  host: www.synsense.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aictx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for aiCTX (now SynSense), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: aiCTX (now SynSense)
provider_slug: aictx
slug: aictx-domain-security
source_filename: aictx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.synsense.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 06:43:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: synsense.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aictx/refs/heads/main/security/aictx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Neuromorphic Computing
- Artificial Intelligence
- Semiconductors
- Edge Computing
- Machine-Learning
- Sensors
- IoT
- Open-Source
- Content
---
