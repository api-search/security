---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: overtime.tv
  spf: false
hosts:
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: overtime.tv
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Overtime Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Overtime, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Overtime
provider_slug: overtime
slug: overtime-domain-security
source_filename: overtime-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: overtime.tv\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: overtime.tv\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/overtime/refs/heads/main/security/overtime-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Sports
- Media
- Entertainment
- Sports League
- Basketball
- Content
- Gen Z
---
