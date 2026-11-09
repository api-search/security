---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: adbloop.com
  spf: true
hosts:
- cert_expires: Dec 10 06:54:57 2026 GMT
  host: adbloop.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Adbloop Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adbloop, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Adbloop
provider_slug: adbloop-com
slug: adbloop-com-domain-security
source_filename: adbloop-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adbloop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 06:54:57 2026 GMT\n  hsts: false\ndomains:\n- domain: adbloop.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/adbloop-com/security/adbloop-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Advertising
- Marketing
- Automation
- Artificial Intelligence
- Software-as-a-Service
- Company
---
