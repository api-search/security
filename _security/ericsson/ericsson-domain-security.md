---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ericsson.com
  spf: true
hosts:
- cert_expires: Sep 21 14:09:21 2026 GMT
  host: www.ericsson.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ericsson Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ericsson, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ericsson
provider_slug: ericsson
slug: ericsson-domain-security
source_filename: ericsson-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ericsson.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 14:09:21 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: ericsson.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ericsson/refs/heads/main/security/ericsson-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Telecommunications
- Networks
- 5G
- 5G RAN
- 5G Core
- Cloud RAN
- ORAN
- Network APIs
- CAMARA
- Aduna
- Programmable Networks
- Network Exposure
- Telecom Equipment
- Enterprise Wireless
- Private 5G
- OSS BSS
- Vonage
- Cradlepoint
- Sweden
---
