---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: shapesecurity.com
  spf: true
hosts:
- cert_expires: Oct  9 10:03:44 2026 GMT
  host: shapesecurity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shape Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shape Security, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Shape Security
provider_slug: shape-security
slug: shape-security-domain-security
source_filename: shape-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shapesecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 10:03:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: shapesecurity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shape-security/refs/heads/main/security/shape-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Security
- Bot Mitigation
- Fraud Prevention
- Application Security
- Acquired
---
