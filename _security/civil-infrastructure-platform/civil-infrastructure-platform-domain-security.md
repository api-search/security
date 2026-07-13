---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cip-project.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: linuxfoundation.org
  spf: true
hosts:
- cert_expires: Aug 27 19:15:50 2026 GMT
  host: www.cip-project.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 05:06:51 2026 GMT
  host: wiki.linuxfoundation.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Civil Infrastructure Platform Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Civil Infrastructure Platform, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Civil Infrastructure Platform
provider_slug: civil-infrastructure-platform
slug: civil-infrastructure-platform-domain-security
source_filename: civil-infrastructure-platform-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cip-project.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 19:15:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: wiki.linuxfoundation.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 05:06:51 2026 GMT\n  hsts: null\ndomains:\n- domain: cip-project.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: linuxfoundation.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/civil-infrastructure-platform/refs/heads/main/security/civil-infrastructure-platform-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Embedded
- Industrial
- Infrastructure
- Linux
- Linux Foundation
- Long-Term Support
- Open Source
---
