---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: umony.com
  spf: true
hosts:
- cert_expires: Sep 20 22:50:59 2026 GMT
  host: umony.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Umony Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Umony, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Umony
provider_slug: umony
slug: umony-domain-security
source_filename: umony-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: umony.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 22:50:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: umony.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/umony/refs/heads/main/security/umony-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Compliance
- Communications
- Call Recording
- Archiving
- RegTech
- Financial Services
---
