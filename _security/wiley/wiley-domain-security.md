---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wiley.com
  spf: true
hosts:
- cert_expires: Sep 27 22:31:50 2026 GMT
  host: www.wiley.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wiley Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wiley, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Wiley
provider_slug: wiley
slug: wiley-domain-security
source_filename: wiley-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wiley.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 22:31:50 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: wiley.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wiley/refs/heads/main/security/wiley-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Publishing
- Education
- Academic
- Research
---
