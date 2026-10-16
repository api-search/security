---
api_specs:
- filename: brink-commerce-openapi-generated.yml
  format: yaml
  label: Brink Commerce API
  slug: brink-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brink-commerce/refs/heads/main/openapi/_ae-authored/brink-commerce-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: brinkcommerce.com
  spf: true
hosts:
- cert_expires: Jan  5 05:24:30 2027 GMT
  host: brinkcommerce.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Brink Commerce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brink Commerce, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Brink Commerce
provider_slug: brink-commerce
slug: brink-commerce-domain-security
source_filename: brink-commerce-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brinkcommerce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 05:24:30 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: brinkcommerce.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brink-commerce/refs/heads/main/security/brink-commerce-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- eCommerce
- API
- Platform
- Enterprise
- Composable
---
