---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: inevitabletech.com
  spf: true
hosts:
- cert_expires: Sep 22 22:06:14 2026 GMT
  host: inevitabletech.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Inevitable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Inevitable, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Inevitable
provider_slug: inevitable
slug: inevitable-domain-security
source_filename: inevitable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: inevitabletech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 22:06:14 2026 GMT\n  hsts: false\ndomains:\n- domain: inevitabletech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inevitable/refs/heads/main/security/inevitable-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Ai Ml
---
