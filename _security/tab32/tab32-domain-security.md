---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tab32.com
  spf: true
hosts:
- cert_expires: Aug 12 18:21:29 2026 GMT
  host: tab32.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tab32 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for tab32, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: tab32
provider_slug: tab32
slug: tab32-domain-security
source_filename: tab32-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tab32.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 18:21:29 2026 GMT\n  hsts: false\ndomains:\n- domain: tab32.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tab32/refs/heads/main/security/tab32-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Dental
- Practice Management
- Healthcare
- Cloud Dental Software
- DSO
- HIPAA
- Patient Data
- Partner API
---
