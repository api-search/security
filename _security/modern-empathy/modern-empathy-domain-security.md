---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: modernempathy.com
  spf: false
hosts:
- cert_expires: Sep  5 19:02:07 2026 GMT
  host: www.modernempathy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Modern Empathy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Modern Empathy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Modern Empathy
provider_slug: modern-empathy
slug: modern-empathy-domain-security
source_filename: modern-empathy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.modernempathy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 19:02:07 2026 GMT\n  hsts: false\ndomains:\n- domain: modernempathy.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modern-empathy/refs/heads/main/security/modern-empathy-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
