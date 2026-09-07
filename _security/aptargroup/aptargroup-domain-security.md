---
api_specs:
- filename: aptargroup-orders-api-openapi.yml
  format: yaml
  label: AptarGroup Orders API
  slug: aptargroup-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aptargroup/refs/heads/main/openapi/aptargroup-orders-api-openapi.yml
- filename: aptargroup-products-api-openapi.yml
  format: yaml
  label: AptarGroup Products API
  slug: aptargroup-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aptargroup/refs/heads/main/openapi/aptargroup-products-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aptar.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aptargroup.com
  spf: true
hosts:
- cert_expires: Oct 31 21:30:39 2026 GMT
  host: www.aptar.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.aptargroup.com
  https: false
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Aptargroup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AptarGroup, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AptarGroup
provider_slug: aptargroup
slug: aptargroup-domain-security
source_filename: aptargroup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aptar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 21:30:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.aptargroup.com\n  https: false\ndomains:\n- domain: aptar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: aptargroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aptargroup/refs/heads/main/security/aptargroup-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Packaging
- Dispensing
- Manufacturing
- Sustainability
- Consumer Goods
- Fortune 1000
---
