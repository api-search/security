---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bitvisual.com.br
  spf: true
hosts:
- cert_expires: Jan  7 15:40:35 2027 GMT
  host: bitvisual.com.br
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bitvisual Com Br Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BitVisual Comunicação Visual, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BitVisual Comunicação Visual
provider_slug: bitvisual-com-br
slug: bitvisual-com-br-domain-security
source_filename: bitvisual-com-br-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bitvisual.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 15:40:35 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bitvisual.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/bitvisual-com-br/security/bitvisual-com-br-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Visual Design
- Print Shop
- Graphic Design
- São Paulo
- Premium Services
---
