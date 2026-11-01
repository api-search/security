---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mylarcomics.com
  spf: false
hosts:
- cert_expires: Dec 31 04:34:33 2026 GMT
  host: mylarcomics.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mylar3 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mylar3, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Mylar3
provider_slug: mylar3
slug: mylar3-domain-security
source_filename: mylar3-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mylarcomics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 04:34:33 2026 GMT\n  hsts: false\ndomains:\n- domain: mylarcomics.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/mylar3/security/mylar3-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Data-Analytics
- Visualization
- Machine-Learning
- APIs
---
