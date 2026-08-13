---
api_specs:
- filename: epsilon-retail-media-integration-openapi.json
  format: json
  label: Epsilon Retail Media Integration API
  slug: epsilon-retail-media-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epsilon/refs/heads/main/openapi/epsilon-retail-media-integration-openapi.json
- filename: epsilon-retail-media-filter-mapping-openapi.json
  format: json
  label: Epsilon Retail Media Filter Mapping API
  slug: epsilon-retail-media-filter-mapping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epsilon/refs/heads/main/openapi/epsilon-retail-media-filter-mapping-openapi.json
- filename: epsilon-retail-media-cross-sell-category-openapi.json
  format: json
  label: Epsilon Retail Media Cross-Sell Category API
  slug: epsilon-retail-media-cross-sell-category-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epsilon/refs/heads/main/openapi/epsilon-retail-media-cross-sell-category-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: epsilon.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: citrusad.com
  spf: true
hosts:
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: epsilon.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 20 05:43:03 2026 GMT
  host: developers.citrusad.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 14:44:06 2026 GMT
  host: eu-ads.rmn.dotomi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Epsilon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Epsilon, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Epsilon
provider_slug: epsilon
slug: epsilon-domain-security
source_filename: epsilon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: epsilon.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: false\n- host: developers.citrusad.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 05:43:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: eu-ads.rmn.dotomi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 14:44:06 2026 GMT\n  hsts: null\ndomains:\n- domain: epsilon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: citrusad.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/epsilon/refs/heads/main/security/epsilon-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Marketing
- Advertising
- Retail Media
- Advertising Technology
- Identity Resolution
- Customer Data
- Loyalty
- Retail
- Publicis Groupe
---
