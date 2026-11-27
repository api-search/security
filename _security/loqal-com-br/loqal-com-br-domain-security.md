---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: loqal.com.br
  spf: true
hosts:
- cert_expires: Jan 13 20:01:24 2027 GMT
  host: loqal.com.br
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Loqal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Loqal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Loqal
provider_slug: loqal-com-br
slug: loqal-com-br-domain-security
source_filename: loqal-com-br-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: loqal.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 20:01:24 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: loqal.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/loqal-com-br/security/loqal-com-br-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Marketplace
- Services
- Brazil
- Artificial Intelligence
- Home Repair
---
