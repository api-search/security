---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: linuxboot.org
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: u-root.org
  spf: false
hosts:
- cert_expires: Sep 26 08:03:22 2026 GMT
  host: www.linuxboot.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 10:47:19 2026 GMT
  host: u-root.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Linuxboot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LinuxBoot, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: LinuxBoot
provider_slug: linuxboot
slug: linuxboot-domain-security
source_filename: linuxboot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.linuxboot.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 08:03:22 2026 GMT\n  hsts: false\n- host: u-root.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 10:47:19 2026 GMT\n  hsts: false\ndomains:\n- domain: linuxboot.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: u-root.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linuxboot/refs/heads/main/security/linuxboot-domain-security.yml
summary_line: TLSv1.3
tags:
- Boot
- Firmware
- Hardware
- Linux Foundation
- u-root
- UEFI
---
