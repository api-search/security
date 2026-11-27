---
api_specs:
- filename: packagento-com-openapi-generated.yml
  format: yaml
  label: Packagento API
  slug: packagento-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/packagento-com/openapi/_ae-authored/packagento-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: packagento.com
  spf: true
hosts:
- cert_expires: Jan  3 07:18:59 2027 GMT
  host: packagento.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Packagento Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Packagento, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Packagento
provider_slug: packagento-com
slug: packagento-com-domain-security
source_filename: packagento-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: packagento.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 07:18:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: packagento.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/packagento-com/security/packagento-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Marketplace
- Magento
- Composer
- PHP
- E-Commerce
---
