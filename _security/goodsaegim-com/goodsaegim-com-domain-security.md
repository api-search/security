---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: goodsaegim.com
  spf: false
hosts:
- cert_expires: Dec 18 02:49:56 2026 GMT
  host: goodsaegim.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 굿새김 GOODSAEGIM Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 굿새김 GOODSAEGIM, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: 굿새김 GOODSAEGIM
provider_slug: goodsaegim-com
slug: goodsaegim-com-domain-security
source_filename: goodsaegim-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: goodsaegim.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 02:49:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: goodsaegim.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/goodsaegim-com/security/goodsaegim-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
