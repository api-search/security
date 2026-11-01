---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ezviz.com
  spf: true
hosts:
- cert_expires: Apr  4 05:31:30 2027 GMT
  host: ezviz.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ezviz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EZVIZ, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: EZVIZ
provider_slug: ezviz
slug: ezviz-domain-security
source_filename: ezviz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ezviz.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Apr  4 05:31:30 2027 GMT\n  hsts: null\ndomains:\n- domain: ezviz.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/ezviz/security/ezviz-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Security Cameras
- Smart Home
- Smart Entry
- Smart Home Appliance
- CloudPlay
- Home Automation
---
