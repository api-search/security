---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: across.to
  spf: true
hosts:
- cert_expires: Sep 29 19:27:48 2026 GMT
  host: across.to
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 08:51:23 2026 GMT
  host: docs.across.to
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 18:44:05 2026 GMT
  host: app.across.to
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Across Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Across, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Across
provider_slug: across
slug: across-domain-security
source_filename: across-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: across.to\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 19:27:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.across.to\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 08:51:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.across.to\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 18:44:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: across.to\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/across/refs/heads/main/security/across-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto Infrastructure
- Cross Chain
- Bridge
- Interoperability
- Blockchain
- DeFi
- Web3
- Swap
- Payments
---
