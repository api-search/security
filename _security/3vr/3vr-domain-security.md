---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: 3vr.com
  spf: true
hosts:
- cert_expires: Mar 14 23:59:59 2027 GMT
  host: 3vr.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 3Vr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 3VR, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: 3VR
provider_slug: 3vr
slug: 3vr-domain-security
source_filename: 3vr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 3vr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 14 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: 3vr.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/3vr/refs/heads/main/security/3vr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Enterprise
- Video Analytics
- Video Surveillance
- Physical Security
- Facial Recognition
- Security
---
