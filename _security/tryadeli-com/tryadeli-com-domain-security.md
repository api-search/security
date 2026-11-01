---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tryadeli.com
  spf: true
hosts:
- cert_expires: Dec  8 14:53:30 2026 GMT
  host: tryadeli.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tryadeli Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adeli, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Adeli
provider_slug: tryadeli-com
slug: tryadeli-com-domain-security
source_filename: tryadeli-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tryadeli.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 14:53:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tryadeli.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/tryadeli-com/security/tryadeli-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Social Media
- Advertising
- API
- Marketing
- Automation
---
