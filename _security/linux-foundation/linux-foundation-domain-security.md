---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: linuxfoundation.org
  spf: true
hosts:
- cert_expires: Sep  9 04:42:18 2026 GMT
  host: www.linuxfoundation.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 14:03:52 2026 GMT
  host: lfx.linuxfoundation.org
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Linux Foundation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Linux Foundation, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Linux Foundation
provider_slug: linux-foundation
slug: linux-foundation-domain-security
source_filename: linux-foundation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.linuxfoundation.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 04:42:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: lfx.linuxfoundation.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 14:03:52 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: linuxfoundation.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linux-foundation/refs/heads/main/security/linux-foundation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Linux Foundation
- Nonprofit
- Open Source
- Technology
- LFX
---
