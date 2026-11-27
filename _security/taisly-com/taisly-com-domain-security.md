---
api_specs:
- filename: taisly-com-api-key-management-api-openapi.yml
  format: yaml
  label: Taisly API Key Management API
  slug: taisly-com-api-key-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taisly-com/openapi/taisly-com-api-key-management-api-openapi.yml
- filename: taisly-com-platforms-api-openapi.yml
  format: yaml
  label: Taisly Platforms API
  slug: taisly-com-platforms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taisly-com/openapi/taisly-com-platforms-api-openapi.yml
- filename: taisly-com-posts-api-openapi.yml
  format: yaml
  label: Taisly Posts API
  slug: taisly-com-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taisly-com/openapi/taisly-com-posts-api-openapi.yml
- filename: taisly-com-reposts-api-openapi.yml
  format: yaml
  label: Taisly Reposts API
  slug: taisly-com-reposts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taisly-com/openapi/taisly-com-reposts-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: taisly.com
  spf: true
hosts:
- cert_expires: Jan 21 20:55:40 2027 GMT
  host: taisly.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Taisly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Taisly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Taisly
provider_slug: taisly-com
slug: taisly-com-domain-security
source_filename: taisly-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: taisly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 20:55:40 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: taisly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/taisly-com/security/taisly-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- VideoPosting
- SocialMedia
- Automation
- API
- Scheduling
---
