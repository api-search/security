---
api_specs:
- filename: tindie-openapi.yml
  format: yaml
  label: Tindie API
  slug: tindie-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tindie/refs/heads/main/openapi/tindie-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tindie.com
  spf: true
hosts:
- cert_expires: Sep 18 09:56:29 2026 GMT
  host: www.tindie.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tindie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tindie, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tindie
provider_slug: tindie
slug: tindie-domain-security
source_filename: tindie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tindie.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 09:56:29 2026 GMT\n  hsts: false\ndomains:\n- domain: tindie.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tindie/refs/heads/main/security/tindie-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Marketplace
- Hardware
- Electronics
- Maker
- eCommerce
- Open Source Hardware
- Orders
---
