---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: missyera.com
  spf: false
hosts:
- cert_expires: Feb  5 04:29:33 2027 GMT
  host: missyera.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Miss Yera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Miss Yera, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Miss Yera
provider_slug: missyera-com
slug: missyera-com-domain-security
source_filename: missyera-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: missyera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 04:29:33 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: missyera.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/missyera-com/security/missyera-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Artificial Intelligence
- Consulting
- Peru
- Enterprise
- Automation
---
