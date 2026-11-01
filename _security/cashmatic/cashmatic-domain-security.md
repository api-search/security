---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cashmatic.it
  spf: true
hosts:
- cert_expires: Dec  1 12:52:31 2026 GMT
  host: cashmatic.it
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cashmatic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cashmatic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cashmatic
provider_slug: cashmatic
slug: cashmatic-domain-security
source_filename: cashmatic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cashmatic.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 12:52:31 2026 GMT\n  hsts: false\ndomains:\n- domain: cashmatic.it\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/cashmatic/security/cashmatic-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Payments
- Retail
- Automation
- POS
---
