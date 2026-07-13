---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pinata.cloud
  spf: true
hosts:
- cert_expires: Sep 10 09:13:36 2026 GMT
  host: pinata.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 15:50:35 2026 GMT
  host: docs.pinata.cloud
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 19:26:00 2026 GMT
  host: api.pinata.cloud
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pinata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pinata, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pinata
provider_slug: pinata
slug: pinata-domain-security
source_filename: pinata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pinata.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 09:13:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.pinata.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 15:50:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.pinata.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 19:26:00 2026 GMT\n  hsts: null\ndomains:\n- domain: pinata.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pinata/refs/heads/main/security/pinata-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Web3
- IPFS
- Storage
- Gateway
---
