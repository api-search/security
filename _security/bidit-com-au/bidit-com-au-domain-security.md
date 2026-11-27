---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bidit.com.au
  spf: true
hosts:
- cert_expires: Jan 23 14:05:06 2027 GMT
  host: bidit.com.au
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bidit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bidit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bidit
provider_slug: bidit-com-au
slug: bidit-com-au-domain-security
source_filename: bidit-com-au-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bidit.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 14:05:06 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bidit.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/bidit-com-au/security/bidit-com-au-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- E-Commerce
- Sales
- Retail
- Marketing
- Technology
- Company
---
