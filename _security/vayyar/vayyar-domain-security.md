---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: vayyar.com
  spf: true
hosts:
- cert_expires: Sep 19 16:13:25 2026 GMT
  host: vayyar.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vayyar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vayyar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Vayyar
provider_slug: vayyar
slug: vayyar-domain-security
source_filename: vayyar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vayyar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 16:13:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vayyar.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vayyar/refs/heads/main/security/vayyar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Deep Tech
- Sensors
- Radar
- Imaging
- IoT
- Hardware
- Elder Care
- Automotive
---
