---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: classcompanion.com
  spf: true
hosts:
- cert_expires: Sep 16 05:13:41 2026 GMT
  host: classcompanion.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Class Companion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Class Companion, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Class Companion
provider_slug: class-companion
slug: class-companion-domain-security
source_filename: class-companion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: classcompanion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 05:13:41 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: classcompanion.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/class-companion/refs/heads/main/security/class-companion-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Ai Ml
---
