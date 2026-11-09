---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: designmaster.com.br
  spf: true
hosts:
- cert_expires: Jan  8 02:09:17 2027 GMT
  host: designmaster.com.br
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Designmaster Com Br Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DesignMaster, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DesignMaster
provider_slug: designmaster-com-br
slug: designmaster-com-br-domain-security
source_filename: designmaster-com-br-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: designmaster.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 02:09:17 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: designmaster.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/designmaster-com-br/security/designmaster-com-br-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Design
- Web Development
- E-Commerce
- Brazil
- Software
---
