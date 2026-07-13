---
api_specs:
- filename: lavu-poslavu-api.yml
  format: yaml
  label: Lavu (POSLavu) API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lavu/refs/heads/main/openapi/lavu-poslavu-api.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lavu.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: poslavu.com
  spf: true
hosts:
- cert_expires: Aug 11 23:59:40 2026 GMT
  host: lavu.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 23:59:59 2026 GMT
  host: admin.poslavu.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lavu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lavu, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lavu
provider_slug: lavu
slug: lavu-domain-security
source_filename: lavu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lavu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 23:59:40 2026 GMT\n  hsts: false\n- host: admin.poslavu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: lavu.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: poslavu.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lavu/refs/heads/main/security/lavu-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Restaurant
- Point of Sale
- Payments
- Inventory
- Menu Management
---
