---
api_specs:
- filename: 1211holding-com-art-api-openapi.yml
  format: yaml
  label: 1211 Art API
  slug: 1211holding-com-art-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/1211holding-com/openapi/1211holding-com-art-api-openapi.yml
- filename: 1211holding-com-catalog-api-openapi.yml
  format: yaml
  label: 1211 Catalog API
  slug: 1211holding-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/1211holding-com/openapi/1211holding-com-catalog-api-openapi.yml
- filename: 1211holding-com-designs-api-openapi.yml
  format: yaml
  label: 1211 Designs API
  slug: 1211holding-com-designs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/1211holding-com/openapi/1211holding-com-designs-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 1211holding.com
  spf: true
hosts:
- cert_expires: Dec 17 01:23:44 2026 GMT
  host: 1211holding.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 1211 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 1211, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: '1211'
provider_slug: 1211holding-com
slug: 1211holding-com-domain-security
source_filename: 1211holding-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 1211holding.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 01:23:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: 1211holding.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/1211holding-com/security/1211holding-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Print on Demand
- E-Commerce
- Merchandise
- Custom Products
---
