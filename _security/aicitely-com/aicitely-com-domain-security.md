---
api_specs:
- filename: aicitely-com-health-api-openapi.yml
  format: yaml
  label: Citely Health API
  slug: aicitely-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aicitely-com/openapi/aicitely-com-health-api-openapi.yml
- filename: aicitely-com-public-api-openapi.yml
  format: yaml
  label: Citely Public API
  slug: aicitely-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aicitely-com/openapi/aicitely-com-public-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: aicitely.com
  spf: true
hosts:
- cert_expires: Dec 14 20:02:56 2026 GMT
  host: aicitely.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Citely Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Citely, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Citely
provider_slug: aicitely-com
slug: aicitely-com-domain-security
source_filename: aicitely-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aicitely.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 20:02:56 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: aicitely.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/aicitely-com/security/aicitely-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- BrandCitation
- SEO
- Analytics
---
