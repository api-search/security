---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: angiodroid.com
  spf: true
hosts:
- cert_expires: Nov 19 16:25:28 2026 GMT
  host: www.angiodroid.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Angiodroid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Angiodroid, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Angiodroid
provider_slug: angiodroid
slug: angiodroid-domain-security
source_filename: angiodroid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.angiodroid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 16:25:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: angiodroid.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/angiodroid/refs/heads/main/security/angiodroid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Medical Technology
- CO2 Imaging
- Vascular Surgery
- Interventional Radiology
---
