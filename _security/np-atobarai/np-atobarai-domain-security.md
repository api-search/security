---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: np-atobarai.jp
  spf: false
hosts:
- cert_expires: May  8 23:59:59 2027 GMT
  host: np-atobarai.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Np Atobarai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NP Atobarai (Net Protections), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: NP Atobarai (Net Protections)
provider_slug: np-atobarai
slug: np-atobarai-domain-security
source_filename: np-atobarai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: np-atobarai.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May  8 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: np-atobarai.jp\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/np-atobarai/security/np-atobarai-domain-security.yml
summary_line: TLSv1.3
tags:
- Fintech
- Payments
- Japan
- Post-pay
- Consumer
---
