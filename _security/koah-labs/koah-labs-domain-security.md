---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: koahlabs.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: koah.ai
  spf: false
hosts:
- cert_expires: Aug 25 19:20:10 2026 GMT
  host: www.koahlabs.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 23:13:12 2026 GMT
  host: docs.koahlabs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 04:54:31 2026 GMT
  host: app.koah.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Koah Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Koah Labs, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Koah Labs
provider_slug: koah-labs
slug: koah-labs-domain-security
source_filename: koah-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.koahlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 19:20:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.koahlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 23:13:12 2026 GMT\n  hsts: false\n- host: app.koah.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 04:54:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: koahlabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: koah.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/koah-labs/refs/heads/main/security/koah-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Advertising
- Ad Network
- Monetization
- Conversion Tracking
- SDKs
- Agents
---
