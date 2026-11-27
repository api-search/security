---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: woundzoom.com
  spf: true
hosts:
- cert_expires: Jan 13 05:40:01 2027 GMT
  host: woundzoom.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: WoundZoom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WoundZoom, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: WoundZoom
provider_slug: woundzoom
slug: woundzoom-domain-security
source_filename: woundzoom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: woundzoom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 05:40:01 2027 GMT\n  hsts: false\ndomains:\n- domain: woundzoom.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/woundzoom/security/woundzoom-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Wound Care
- Healthcare Software
- Hospitals
- Long-Term Care
- Home Care
- EHR Integration
---
