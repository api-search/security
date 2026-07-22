---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: lf.co
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lightforceortho.com
  spf: true
hosts:
- cert_expires: Sep 23 15:50:13 2026 GMT
  host: lf.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 02:07:39 2026 GMT
  host: id.lightforceortho.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lightforce Orthodontics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LightForce Orthodontics, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: LightForce Orthodontics
provider_slug: lightforce-orthodontics
slug: lightforce-orthodontics-domain-security
source_filename: lightforce-orthodontics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lf.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 15:50:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: id.lightforceortho.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 02:07:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lf.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: lightforceortho.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightforce-orthodontics/refs/heads/main/security/lightforce-orthodontics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Orthodontics
- Medical Devices
- Dental
- 3D Printing
- Manufacturing
- Identity
---
