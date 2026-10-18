---
api_specs:
- filename: deepinquiry-facts-api-openapi.yml
  format: yaml
  label: DeepInquiry Verified Facts API (Machine Accountability Corp) Facts API
  slug: deepinquiry-facts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepinquiry/refs/heads/main/openapi/deepinquiry-facts-api-openapi.yml
- filename: deepinquiry-search-api-openapi.yml
  format: yaml
  label: DeepInquiry Verified Facts API (Machine Accountability Corp) Search API
  slug: deepinquiry-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepinquiry/refs/heads/main/openapi/deepinquiry-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: deepinquiry.ai
  spf: true
hosts:
- cert_expires: Nov 26 17:20:12 2026 GMT
  host: www.deepinquiry.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Deepinquiry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DeepInquiry Verified Facts API (Machine Accountability Corp), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DeepInquiry Verified Facts API (Machine Accountability Corp)
provider_slug: deepinquiry
slug: deepinquiry-domain-security
source_filename: deepinquiry-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.deepinquiry.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 17:20:12 2026 GMT\n  hsts: null\ndomains:\n- domain: deepinquiry.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deepinquiry/refs/heads/main/security/deepinquiry-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- API
- Facts
- Verification
- Data
---
