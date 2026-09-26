---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: angeleyehealth.com
  spf: true
hosts:
- cert_expires: Nov 26 04:40:04 2026 GMT
  host: www.angeleyehealth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Angeleyecamerasystems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Angeleyecamerasystems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Angeleyecamerasystems
provider_slug: angeleyecamerasystems
slug: angeleyecamerasystems-domain-security
source_filename: angeleyecamerasystems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.angeleyehealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 04:40:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: angeleyehealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/angeleyecamerasystems/refs/heads/main/security/angeleyecamerasystems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- NICU
- Camera System
- Feeding Management
- Hospital Solutions
---
