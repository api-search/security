---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: caretlegal.com
  spf: true
hosts:
- cert_expires: Jan  6 06:17:53 2027 GMT
  host: caretlegal.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Caret Legal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CARET Legal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CARET Legal
provider_slug: caret-legal
slug: caret-legal-domain-security
source_filename: caret-legal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: caretlegal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 06:17:53 2027 GMT\n  hsts: false\ndomains:\n- domain: caretlegal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/caret-legal/security/caret-legal-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- LegalTech
- SaaS
- Cloud
- PracticeManagement
---
