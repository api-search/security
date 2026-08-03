---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: echodyne.com
  spf: true
hosts:
- cert_expires: Sep 18 01:29:57 2026 GMT
  host: www.echodyne.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 22 15:25:46 2027 GMT
  host: portal.echodyne.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Echodyne Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Echodyne, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Echodyne
provider_slug: echodyne
slug: echodyne-domain-security
source_filename: echodyne-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.echodyne.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 01:29:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: portal.echodyne.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 15:25:46 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: echodyne.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/echodyne/refs/heads/main/security/echodyne-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Radar
- Defense
- Government
- Critical Infrastructure
- Counter-UAS
- Drone Detection
- Sensors
- Situational Awareness
- Aerospace
- Hardware
- Public Safety
---
