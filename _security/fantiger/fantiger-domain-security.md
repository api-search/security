---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fantiger.com
  spf: false
hosts:
- cert_expires: Sep 29 12:04:49 2026 GMT
  host: fantiger.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fantiger Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fantiger, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Fantiger
provider_slug: fantiger
slug: fantiger-domain-security
source_filename: fantiger-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fantiger.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 12:04:49 2026 GMT\n  hsts: null\ndomains:\n- domain: fantiger.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fantiger/refs/heads/main/security/fantiger-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Crypto Web3
---
