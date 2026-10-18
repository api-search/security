---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: distillsync.com
  spf: true
hosts:
- cert_expires: Dec 12 08:19:48 2026 GMT
  host: distillsync.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Distillsync Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Distillsync, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Distillsync
provider_slug: distillsync
slug: distillsync-domain-security
source_filename: distillsync-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: distillsync.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 08:19:48 2026 GMT\n  hsts: false\ndomains:\n- domain: distillsync.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/distillsync/refs/heads/main/security/distillsync-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Integration
- ERP
- E-Commerce
- Automation
---
