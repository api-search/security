---
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: false
  dnssec: true
  domain: servo.org
  spf: true
hosts:
- cert_expires: Aug 21 07:31:33 2026 GMT
  host: servo.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Servo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Servo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Servo
provider_slug: servo
slug: servo-domain-security
source_filename: servo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: servo.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 07:31:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: servo.org\n  dnssec: true\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/servo/refs/heads/main/security/servo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Browser
- Linux Foundation
- Rust
- Web Engine
---
