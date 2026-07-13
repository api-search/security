---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: keyrunner.app
  spf: false
hosts:
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: keyrunner.app
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Keyrunner Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KeyRunner, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: KeyRunner
provider_slug: keyrunner
slug: keyrunner-domain-security
source_filename: keyrunner-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: keyrunner.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: keyrunner.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keyrunner/refs/heads/main/security/keyrunner-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- API Client
- API Testing
- Developer Tools
- Local-First
- Mock Server
- Secret Management
---
