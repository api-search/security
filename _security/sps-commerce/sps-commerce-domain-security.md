---
api_specs:
- filename: sps-commerce-submission-api-openapi.yml
  format: yaml
  label: SPS Commerce Trading Partner Submission API
  slug: sps-commerce-trading-partner-submission-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sps-commerce/refs/heads/main/openapi/sps-commerce-submission-api-openapi.yml
- filename: sps-commerce-inventory-api-openapi.yml
  format: yaml
  label: SPS Commerce Inventory API
  slug: sps-commerce-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sps-commerce/refs/heads/main/openapi/sps-commerce-inventory-api-openapi.yml
- filename: sps-commerce-import-api-openapi.yml
  format: yaml
  label: SPS Commerce Import API
  slug: sps-commerce-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sps-commerce/refs/heads/main/openapi/sps-commerce-import-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: spscommerce.com
  spf: true
hosts:
- cert_expires: Oct 31 16:23:15 2026 GMT
  host: www.spscommerce.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sps Commerce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SPS Commerce, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SPS Commerce
provider_slug: sps-commerce
slug: sps-commerce-domain-security
source_filename: sps-commerce-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.spscommerce.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 31 16:23:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\ndomains:\n- domain: spscommerce.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sps-commerce/refs/heads/main/security/sps-commerce-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- EDI
- Retail
- Supply Chain
- Commerce
- Trading Partners
- API Standards
---
