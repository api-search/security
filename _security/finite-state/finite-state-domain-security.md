---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: finitestate.io
  spf: true
hosts:
- cert_expires: Sep 20 05:33:16 2026 GMT
  host: finitestate.io
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 63072000
  hsts_preload: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 12:53:47 2026 GMT
  host: app.finitestate.io
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 63072000
  hsts_preload: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: docs.finitestate.io
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: platform.finitestate.io
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Finite State Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Finite State, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Finite State
provider_slug: finite-state
slug: finite-state-domain-security
source_filename: finite-state-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts (0-working/probe-domain-security.py,\n  then hand-verified with curl and openssl s_client on 2026-08-04)\nnote: 'The mechanical probe reported hsts: null for every host and omitted\n  platform.finitestate.io. Both were corrected against direct HEAD and GET\n  observations: all four hosts return a Strict-Transport-Security header.'\nhosts:\n- host: finitestate.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 05:33:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: false\n  hsts_preload: false\n- host: app.finitestate.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 12:53:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: false\n  hsts_preload: false\n- host: docs.finitestate.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n\
  \  hsts_include_subdomains: true\n  hsts_preload: false\n- host: platform.finitestate.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: false\ndomains:\n- domain: finitestate.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\nfindings:\n- id: no-caa\n  severity: low\n  detail: no CAA record is published for finitestate.io, so certificate issuance is\n    not restricted to named CAs\n- id: no-dnssec\n  severity: low\n  detail: DNSSEC is not enabled on finitestate.io\n- id: tls12-on-platform-hosts\n  severity: informational\n  detail: docs.finitestate.io and platform.finitestate.io negotiated TLSv1.2 while\n    finitestate.io and app.finitestate.io negotiated TLSv1.3\n- id: dmarc-reject\n  severity: positive\n  detail: DMARC is published with p=reject, the strongest policy\n- id: no-security-txt\n  severity: medium\n  detail: no RFC\
  \ 9116 security.txt on any host, and no vulnerability-disclosure or\n    trust page was found — a notable gap for a product security vendor\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finite-state/refs/heads/main/security/finite-state-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Product Security
- Software Supply Chain Security
- SBOM
- Firmware Analysis
- Vulnerability Management
- Binary Analysis
- Connected Devices
- Compliance
- Cybersecurity
- IoT
---
