---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: helium.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hellohelium.com
  spf: true
hosts:
- cert_expires: Aug 28 07:56:33 2026 GMT
  host: www.helium.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 19:04:43 2026 GMT
  host: www.hellohelium.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 20:09:20 2026 GMT
  host: docs.helium.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Helium Network Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Helium Network, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Helium Network
provider_slug: helium-network
slug: helium-network-domain-security
source_filename: helium-network-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.helium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 07:56:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.hellohelium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 19:04:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.helium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 20:09:20 2026 GMT\n  hsts: false\ndomains:\n- domain: helium.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: hellohelium.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/helium-network/refs/heads/main/security/helium-network-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Wireless
- IoT
- LoRaWAN
- 5G
- DePIN
- Solana
- Crypto
---
