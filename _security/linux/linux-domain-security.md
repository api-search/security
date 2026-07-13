---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kernel.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: linuxfoundation.org
  spf: true
hosts:
- cert_expires: Oct 18 00:52:15 2026 GMT
  host: www.kernel.org
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 04:42:18 2026 GMT
  host: www.linuxfoundation.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 19:55:29 2026 GMT
  host: man7.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Linux Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Linux, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Linux
provider_slug: linux
slug: linux-domain-security
source_filename: linux-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kernel.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 00:52:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: www.linuxfoundation.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 04:42:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: man7.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 19:55:29 2026 GMT\n  hsts: false\ndomains:\n- domain: kernel.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: linuxfoundation.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linux/refs/heads/main/security/linux-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Kernel
- Linux
- Open Source
- Operating System
- Unix
- Userspace API
---
