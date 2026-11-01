---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: fakto.app
  spf: true
hosts:
- cert_expires: Dec 26 18:54:58 2026 GMT
  host: fakto.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fakto App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for fakto-app, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: fakto-app
provider_slug: fakto-app
slug: fakto-app-domain-security
source_filename: fakto-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fakto.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 18:54:58 2026 GMT\n  hsts: false\ndomains:\n- domain: fakto.app\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/fakto-app/security/fakto-app-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- AI
- Accounting
- Integration
- Poland
- Automation
---
