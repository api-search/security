---
api_specs:
- filename: esim-global-vip-openapi.json
  format: json
  label: eSIM Catalog
  slug: esim-catalog
  spec_type: OpenAPI
  url: https://artifacts.apis.io/esim-global-vip/openapi/esim-global-vip-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: esim-global.vip
  spf: true
hosts:
- cert_expires: Feb  4 00:06:50 2027 GMT
  host: esim-global.vip
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: eSIM-Global.VIP Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for eSIM-Global.VIP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: eSIM-Global.VIP
provider_slug: esim-global-vip
slug: esim-global-vip-domain-security
source_filename: esim-global-vip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: esim-global.vip\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 00:06:50 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: esim-global.vip\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/esim-global-vip/security/esim-global-vip-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- eSIM
- Travel
- Telecommunications
- Prepaid
---
