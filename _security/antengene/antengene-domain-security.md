---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: antengene.com
  spf: true
hosts:
- cert_expires: Oct  3 08:19:05 2026 GMT
  host: antengene.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Antengene Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for antengene, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: antengene
provider_slug: antengene
slug: antengene-domain-security
source_filename: antengene-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: antengene.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 08:19:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: antengene.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/antengene/refs/heads/main/security/antengene-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Biopharmaceutical
- Oncology
- Pharmaceuticals
- Healthcare
- Life Sciences
- Drug Development
---
