---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: datawebot.com
  spf: true
hosts:
- cert_expires: Jan 11 08:46:26 2027 GMT
  host: datawebot.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: datawebot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for datawebot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: datawebot
provider_slug: datawebot-com
slug: datawebot-com-domain-security
source_filename: datawebot-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datawebot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 08:46:26 2027 GMT\n  hsts: false\ndomains:\n- domain: datawebot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/datawebot-com/security/datawebot-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- E-Commerce
- Artificial Intelligence
- Data
- Marketplace
---
