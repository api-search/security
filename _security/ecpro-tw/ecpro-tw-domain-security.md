---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ecpro.tw
  spf: true
hosts:
- cert_expires: Dec 13 09:43:32 2026 GMT
  host: ecpro.tw
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ECPRO Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ECPRO, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ECPRO
provider_slug: ecpro-tw
slug: ecpro-tw-domain-security
source_filename: ecpro-tw-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ecpro.tw\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 09:43:32 2026 GMT\n  hsts: false\ndomains:\n- domain: ecpro.tw\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ecpro-tw/security/ecpro-tw-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- E-Commerce
- Data
- Taiwan
- Media
---
