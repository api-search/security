---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: transparentsystems.com
  spf: true
hosts:
- cert_expires: Sep 13 20:20:37 2026 GMT
  host: www.transparentsystems.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Transparent Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Transparent Systems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Transparent Systems
provider_slug: transparent-systems
slug: transparent-systems-domain-security
source_filename: transparent-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nnote: transparentsystems.com is a parked GoDaddy for-sale lander (307 to forsale.godaddy.com,\n  null MX, wildcard 200s) as of 2026-07-21 — this records the parking host's posture,\n  not live company infrastructure. The company appears defunct.\nhosts:\n- host: www.transparentsystems.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 20:20:37 2026 GMT\n  hsts: false\ndomains:\n- domain: transparentsystems.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transparent-systems/refs/heads/main/security/transparent-systems-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Crypto
- Fintech
- Payments
- Settlement
- Blockchain
- Defunct
---
