---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: laraue.com
  spf: true
hosts:
- cert_expires: Feb  8 19:50:22 2027 GMT
  host: laraue.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Laraue Software Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Laraue Software, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Laraue Software
provider_slug: laraue-com
slug: laraue-com-domain-security
source_filename: laraue-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: laraue.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 19:50:22 2027 GMT\n  hsts: false\ndomains:\n- domain: laraue.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/laraue-com/security/laraue-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Software
- Productivity
- Tools
- Developers
---
