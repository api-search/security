---
api_specs:
- filename: graunt-com-openapi-generated.yml
  format: yaml
  label: Graunt API
  slug: graunt-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/graunt-com/openapi/_ae-authored/graunt-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: graunt.com
  spf: true
hosts:
- cert_expires: Apr  1 23:59:59 2027 GMT
  host: graunt.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Graunt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Graunt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Graunt
provider_slug: graunt-com
slug: graunt-com-domain-security
source_filename: graunt-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: graunt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: graunt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/graunt-com/security/graunt-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Data Marketplace
- Marketplace
- Data
---
