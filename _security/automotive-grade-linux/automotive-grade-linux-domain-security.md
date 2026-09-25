---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: automotivelinux.org
  spf: true
hosts:
- cert_expires: Nov  5 17:59:39 2026 GMT
  host: www.automotivelinux.org
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 09:46:33 2026 GMT
  host: docs.automotivelinux.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 27 17:07:36 2026 GMT
  host: lava.automotivelinux.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Automotive Grade Linux Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Automotive Grade Linux, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Automotive Grade Linux
provider_slug: automotive-grade-linux
slug: automotive-grade-linux-domain-security
source_filename: automotive-grade-linux-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.automotivelinux.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 17:59:39 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: docs.automotivelinux.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 09:46:33 2026 GMT\n  hsts: false\n- host: lava.automotivelinux.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 17:07:36 2026 GMT\n  hsts: false\ndomains:\n- domain: automotivelinux.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/automotive-grade-linux/refs/heads/main/security/automotive-grade-linux-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automotive
- Connected Vehicles
- Embedded Linux
- In-Vehicle Infotainment
- IoT
- Linux Foundation
- Open Source
- Software Defined Vehicles
---
