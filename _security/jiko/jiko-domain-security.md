---
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: jiko.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: jiko.io
  spf: true
hosts:
- cert_expires: Sep 21 12:03:52 2026 GMT
  host: jiko.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: business.jiko.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 00:59:03 2026 GMT
  host: docs.jiko.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jiko Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jiko, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Jiko
provider_slug: jiko
slug: jiko-domain-security
source_filename: jiko-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jiko.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 12:03:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: business.jiko.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: null\n- host: docs.jiko.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 00:59:03 2026 GMT\n  hsts: false\ndomains:\n- domain: jiko.com\n  dnssec: true\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: jiko.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jiko/refs/heads/main/security/jiko-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Banking
- Payments
- Treasury
- Embedded Finance
- Fintech
- Cards
- Settlement
- Broker-Dealer
- Banking as a Service
---
