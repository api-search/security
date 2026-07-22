---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aireye.tech
  spf: true
hosts:
- cert_expires: Sep 14 10:22:28 2026 GMT
  host: www.aireye.tech
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aireye Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AirEye, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AirEye
provider_slug: aireye
slug: aireye-domain-security
source_filename: aireye-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aireye.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 10:22:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: aireye.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aireye/refs/heads/main/security/aireye-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Cybersecurity
- Wireless
- Network Security
- Wi-Fi
- Operational Technology
- Threat Detection
---
