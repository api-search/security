---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: evigence.com
  spf: true
hosts:
- cert_expires: Sep 29 19:09:00 2026 GMT
  host: www.evigence.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Evigence Sensors Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Evigence Sensors, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Evigence Sensors
provider_slug: evigence-sensors
slug: evigence-sensors-domain-security
source_filename: evigence-sensors-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.evigence.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 19:09:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: evigence.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evigence-sensors/refs/heads/main/security/evigence-sensors-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Food Technology
- Freshness Monitoring
- Cold Chain
- Sensors
- IoT
- Supply Chain
- Food Safety
---
