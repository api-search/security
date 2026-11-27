---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gammarips.com
  spf: true
hosts:
- cert_expires: Jan 30 12:32:11 2027 GMT
  host: gammarips.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GammaRips Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GammaRips, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: GammaRips
provider_slug: gammarips-com
slug: gammarips-com-domain-security
source_filename: gammarips-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gammarips.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 12:32:11 2027 GMT\n  hsts: false\ndomains:\n- domain: gammarips.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/gammarips-com/security/gammarips-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Options
- AI Trading
- Financial Data
---
