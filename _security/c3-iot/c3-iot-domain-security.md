---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: c3.ai
  spf: true
hosts:
- cert_expires: Dec 12 15:56:01 2026 GMT
  host: www.c3.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: C3 Iot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for C3.ai (C3 IoT), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: C3.ai (C3 IoT)
provider_slug: c3-iot
slug: c3-iot-domain-security
source_filename: c3-iot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.c3.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 15:56:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: c3.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/c3-iot/refs/heads/main/security/c3-iot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Enterprise
- Platform
- IoT
- Industry
---
