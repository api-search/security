---
api_specs:
- filename: curie-openapi.json
  format: json
  label: Curie 3D Product Commerce API
  slug: curie-3d-product-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curie/refs/heads/main/openapi/curie-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: curie.co
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: curie.app
  spf: false
hosts:
- cert_expires: Oct 11 00:24:35 2026 GMT
  host: curie.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 01:55:41 2026 GMT
  host: chat.curie.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 16:48:26 2026 GMT
  host: curie-api.curievision.workers.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Curie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Curie, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Curie
provider_slug: curie
slug: curie-domain-security
source_filename: curie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: curie.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 00:24:35 2026 GMT\n  hsts: false\n- host: chat.curie.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 01:55:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: curie-api.curievision.workers.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 16:48:26 2026 GMT\n  hsts: null\ndomains:\n- domain: curie.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: curie.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/curie/refs/heads/main/security/curie-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Commerce
- E-Commerce
- Shopify
- Artificial Intelligence
- Model Context Protocol
- Agentic Commerce
- Product Discovery
- 3D
---
