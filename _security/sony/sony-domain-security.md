---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sony.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: nnabla.org
  spf: false
hosts:
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: www.sony.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: nnabla.org
  https: false
- cert_expires: Nov 29 23:59:59 2026 GMT
  host: developer.sony.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sony Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sony, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sony
provider_slug: sony
slug: sony-domain-security
source_filename: sony-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sony.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: null\n- host: nnabla.org\n  https: false\n- host: developer.sony.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sony.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: nnabla.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sony/refs/heads/main/security/sony-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Technology
- Consumer Electronics
- Gaming
- Entertainment
- Artificial Intelligence
---
