---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zephyrproject.org
  spf: true
hosts:
- cert_expires: Aug 26 08:38:02 2026 GMT
  host: www.zephyrproject.org
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: docs.zephyrproject.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zephyr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zephyr Project, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Zephyr Project
provider_slug: zephyr
slug: zephyr-domain-security
source_filename: zephyr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zephyrproject.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 08:38:02 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: docs.zephyrproject.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: zephyrproject.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zephyr/refs/heads/main/security/zephyr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Embedded
- IoT
- Linux Foundation
- RTOS
- Open Source
- Edge
---
