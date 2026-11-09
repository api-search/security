---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cartena.com.br
  spf: true
hosts:
- cert_expires: Jan 27 15:02:17 2027 GMT
  host: cartena.com.br
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cartena Com Br Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cartena, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cartena
provider_slug: cartena-com-br
slug: cartena-com-br-domain-security
source_filename: cartena-com-br-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cartena.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 15:02:17 2027 GMT\n  hsts: false\ndomains:\n- domain: cartena.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/cartena-com-br/security/cartena-com-br-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Finance
- Investment
- Portfolio
- Dividends
- Brazil
---
