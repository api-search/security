---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rayzebio.com
  spf: true
hosts:
- cert_expires: Sep 23 12:53:20 2026 GMT
  host: rayzebio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rayzebio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RayzeBio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: RayzeBio
provider_slug: rayzebio
slug: rayzebio-domain-security
source_filename: rayzebio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rayzebio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 12:53:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rayzebio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rayzebio/refs/heads/main/security/rayzebio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Oncology
- Radiopharmaceuticals
- Life Sciences
- Healthcare
- Clinical Trials
- Drug Discovery
---
