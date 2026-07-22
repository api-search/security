---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cemanet.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ansi.org
  spf: true
hosts:
- cert_expires: Sep 27 13:36:09 2026 GMT
  host: cemanet.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 20:13:06 2026 GMT
  host: webstore.ansi.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Belts Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Belts, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Belts
provider_slug: belts
slug: belts-domain-security
source_filename: belts-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cemanet.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 13:36:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: webstore.ansi.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 20:13:06 2026 GMT\n  hsts: null\ndomains:\n- domain: cemanet.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: ansi.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/belts/refs/heads/main/security/belts-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Bulk Material Handling
- Condition Monitoring
- Conveyor Belts
- IIoT
- Industrial Automation
- Manufacturing
- Mining
- Predictive Maintenance
- Sensors
---
