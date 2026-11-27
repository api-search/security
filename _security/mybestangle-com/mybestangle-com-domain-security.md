---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mybestangle.com
  spf: true
hosts:
- cert_expires: Jan 30 13:19:28 2027 GMT
  host: mybestangle.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MyBestAngle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MyBestAngle, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MyBestAngle
provider_slug: mybestangle-com
slug: mybestangle-com-domain-security
source_filename: mybestangle-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mybestangle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 13:19:28 2027 GMT\n  hsts: null\ndomains:\n- domain: mybestangle.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mybestangle-com/security/mybestangle-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Photography
- Image Processing
- Artificial Intelligence
- SelfieEnhancement
- Consumer App
---
