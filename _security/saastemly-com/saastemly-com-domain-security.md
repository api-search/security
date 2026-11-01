---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: saastemly.com
  spf: true
hosts:
- cert_expires: Nov 30 06:01:38 2026 GMT
  host: saastemly.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Saastemly Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for saastemly-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: saastemly-com
provider_slug: saastemly-com
slug: saastemly-com-domain-security
source_filename: saastemly-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: saastemly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 06:01:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: saastemly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/saastemly-com/security/saastemly-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Software Development
- Custom Software
- Web Applications
- Mobile Apps
- AI/ML
---
