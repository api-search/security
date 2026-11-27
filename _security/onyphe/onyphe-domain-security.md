---
api_specs:
- filename: onyphe-asd-api-openapi.yml
  format: yaml
  label: ONYPHE ASD API
  slug: onyphe-asd-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onyphe/openapi/onyphe-asd-api-openapi.yml
- filename: onyphe-discovery-api-openapi.yml
  format: yaml
  label: ONYPHE Discovery API
  slug: onyphe-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onyphe/openapi/onyphe-discovery-api-openapi.yml
- filename: onyphe-export-api-openapi.yml
  format: yaml
  label: ONYPHE Export API
  slug: onyphe-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onyphe/openapi/onyphe-export-api-openapi.yml
- filename: onyphe-search-api-openapi.yml
  format: yaml
  label: ONYPHE Search API
  slug: onyphe-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onyphe/openapi/onyphe-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: onyphe.com
  spf: true
hosts:
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: onyphe.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ONYPHE Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ONYPHE, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: ONYPHE
provider_slug: onyphe
slug: onyphe-domain-security
source_filename: onyphe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: onyphe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: onyphe.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/onyphe/security/onyphe-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Attack Surface Management
- Threat Intelligence
- Internet Scanning
- Passive DNS
- Vulnerability Data
---
