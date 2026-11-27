---
api_specs:
- filename: loupe-legal-cite-api-openapi.yml
  format: yaml
  label: Loupe Cite API
  slug: loupe-legal-cite-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/loupe-legal/openapi/loupe-legal-cite-api-openapi.yml
- filename: loupe-legal-coverage-api-openapi.yml
  format: yaml
  label: Loupe Coverage API
  slug: loupe-legal-coverage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/loupe-legal/openapi/loupe-legal-coverage-api-openapi.yml
- filename: loupe-legal-search-api-openapi.yml
  format: yaml
  label: Loupe Search API
  slug: loupe-legal-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/loupe-legal/openapi/loupe-legal-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: loupe.legal
  spf: true
hosts:
- cert_expires: Dec 23 20:41:33 2026 GMT
  host: loupe.legal
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Loupe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Loupe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Loupe
provider_slug: loupe-legal
slug: loupe-legal-domain-security
source_filename: loupe-legal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: loupe.legal\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 20:41:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: loupe.legal\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/loupe-legal/security/loupe-legal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Legal
- Citations
- Artificial Intelligence
- Court-Filing
- Software-as-a-Service
---
