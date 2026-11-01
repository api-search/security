---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bugezy.dev
  spf: false
hosts:
- cert_expires: Jan 24 12:30:20 2027 GMT
  host: bugezy.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bugezy Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for bugezy-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: bugezy-dev
provider_slug: bugezy-dev
slug: bugezy-dev-domain-security
source_filename: bugezy-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bugezy.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 12:30:20 2027 GMT\n  hsts: null\ndomains:\n- domain: bugezy.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/bugezy-dev/security/bugezy-dev-domain-security.yml
summary_line: TLSv1.3
tags:
- BugReporting
- AI
- DeveloperTools
- SaaS
- Productivity
---
