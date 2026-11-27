---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: merchsage.com
  spf: true
hosts:
- cert_expires: Feb  1 09:25:30 2027 GMT
  host: merchsage.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MerchSage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MerchSage, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MerchSage
provider_slug: merchsage-com
slug: merchsage-com-domain-security
source_filename: merchsage-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: merchsage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 09:25:30 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: merchsage.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/merchsage-com/security/merchsage-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Merchandising
- E-Commerce
- YouTube
- Automation
---
