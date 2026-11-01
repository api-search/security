---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: unmanic.app
  spf: false
hosts:
- cert_expires: Dec 29 10:01:21 2026 GMT
  host: unmanic.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Unmanic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unmanic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Unmanic
provider_slug: unmanic
slug: unmanic-domain-security
source_filename: unmanic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: unmanic.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 10:01:21 2026 GMT\n  hsts: false\ndomains:\n- domain: unmanic.app\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/unmanic/security/unmanic-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Media
- Automation
- OpenSource
- FileManagement
- Optimization
---
