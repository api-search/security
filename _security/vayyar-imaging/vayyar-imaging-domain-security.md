---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: vayyar.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: walabot.com
  spf: true
hosts:
- cert_expires: Sep 19 16:13:25 2026 GMT
  host: vayyar.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 00:59:03 2026 GMT
  host: walabot.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vayyar Imaging Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vayyar Imaging, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Vayyar Imaging
provider_slug: vayyar-imaging
slug: vayyar-imaging-domain-security
source_filename: vayyar-imaging-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vayyar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 16:13:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: walabot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 00:59:03 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: vayyar.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: walabot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vayyar-imaging/refs/heads/main/security/vayyar-imaging-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Sensors
- Radar
- Imaging
- IoT
- Healthcare
- Elderly Care
- Automotive
- Smart Home
---
