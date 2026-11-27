---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: metrichub.app
  spf: true
hosts:
- cert_expires: Feb  6 17:59:07 2027 GMT
  host: metrichub.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: mhwork Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for mhwork, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: mhwork
provider_slug: metrichub-app
slug: metrichub-app-domain-security
source_filename: metrichub-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: metrichub.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 17:59:07 2027 GMT\n  hsts: false\ndomains:\n- domain: metrichub.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/metrichub-app/security/metrichub-app-domain-security.yml
summary_line: TLSv1.3
tags:
- Artificial Intelligence
- Automation
- Desktop
- Integration
- Productivity
---
