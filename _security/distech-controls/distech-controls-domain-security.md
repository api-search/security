---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: distech-controls.com
  spf: true
hosts:
- cert_expires: Jan 22 06:57:25 2027 GMT
  host: www.distech-controls.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Distech Controls Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Distech Controls, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Distech Controls
provider_slug: distech-controls
slug: distech-controls-domain-security
source_filename: distech-controls-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.distech-controls.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 06:57:25 2027 GMT\n  hsts: null\ndomains:\n- domain: distech-controls.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/distech-controls/security/distech-controls-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Building Automation
- Control
- Lighting
- Access Control
- Facility Management
- Smart Buildings
---
