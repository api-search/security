---
api_specs:
- filename: productiv-developer-openapi.yml
  format: yaml
  label: Productiv Developer API
  slug: developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/productiv/refs/heads/main/openapi/productiv-developer-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: productiv.com
  spf: true
hosts:
- cert_expires: Jan  3 23:59:59 2027 GMT
  host: docs.app.productiv.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 23:59:59 2026 GMT
  host: public-api.productiv.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: login.api.productiv.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Productiv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Productiv, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Productiv
provider_slug: productiv
slug: productiv-domain-security
source_filename: productiv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.app.productiv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 23:59:59 2027 GMT\n  hsts: false\n- host: public-api.productiv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 23:59:59 2026 GMT\n  hsts: null\n- host: login.api.productiv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: productiv.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/productiv/refs/heads/main/security/productiv-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Application Portfolio
- Provisioning
- SaaS Management
- Spend Management
- Usage Analytics
---
