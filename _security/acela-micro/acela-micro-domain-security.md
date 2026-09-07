---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: acelamicro.com
  mx:
  - 5 mxbiz1.qq.com.
  - 10 mxbiz2.qq.com.
  spf: false
hosts:
- cert_expires: Nov 17 21:11:28 2026 GMT
  cert_issuer: Let's Encrypt (CN=YR2)
  host: www.acelamicro.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- host: acelamicro.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Acela Micro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acela Micro, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Acela Micro
provider_slug: acela-micro
slug: acela-micro-domain-security
source_filename: acela-micro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.acelamicro.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 17 21:11:28 2026 GMT\n  cert_issuer: \"Let's Encrypt (CN=YR2)\"\n  hsts: false\n- host: acelamicro.com\n  https: true\n  tls_version: TLSv1.3\n  hsts: false\ndomains:\n- domain: acelamicro.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  mx:\n  - 5 mxbiz1.qq.com.\n  - 10 mxbiz2.qq.com.\nnotes: >-\n  Probed 2026-09-06 from a US vantage point. The origin (8.159.144.100, Alibaba Cloud, China)\n  is reachable but slow and frequently resets connections from non-browser clients, so the\n  shared probe-domain-security.py 5s timeout reported the host unreachable; these values were\n  collected by re-running that script's own probe functions with a 45s timeout plus openssl\n  s_client and curl. www.acelamicro.com terminates TLS 1.2 with a Let's Encrypt certificate;\n  the\
  \ apex negotiates TLS 1.3. Neither host returns a Strict-Transport-Security header.\n  The registrable domain publishes no DNSSEC, no CAA, no SPF and no DMARC record — an absence\n  confirmed against authoritative DNS, not a probe timeout. Mail is hosted on Tencent QQ\n  Enterprise Mail; with no SPF or DMARC the domain is unprotected against email spoofing.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acela-micro/refs/heads/main/security/acela-micro-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Semiconductors
- Integrated Circuits
- Analog to Digital Converters
- Digital to Analog Converters
- RF Transceivers
- Signal Chain
- Electronic Components
- Hardware
- China
---
