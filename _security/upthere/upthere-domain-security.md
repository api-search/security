---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: upthere.com
  spf: true
hosts:
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: upthere.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Upthere Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Upthere, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Upthere
provider_slug: upthere
slug: upthere-domain-security
source_filename: upthere-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: upthere.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: upthere.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upthere/refs/heads/main/security/upthere-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Consumer
- Cloud Storage
- File Sharing
- Photos
- Media
- Defunct
- Acquired
---
