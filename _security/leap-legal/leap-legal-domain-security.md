---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: leap.us
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: leap.build
  spf: true
hosts:
- cert_expires: Aug 21 00:14:22 2026 GMT
  host: leap.us
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: developer.leap.build
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 02:30:31 2026 GMT
  host: www.leap.build
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Leap Legal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LEAP, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: LEAP
provider_slug: leap-legal
slug: leap-legal-domain-security
source_filename: leap-legal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: leap.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 00:14:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.leap.build\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: false\n- host: www.leap.build\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 02:30:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: leap.us\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: leap.build\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leap-legal/refs/heads/main/security/leap-legal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Legal
- LegalTech
- Practice Management
- Legal Accounting
- Trust Accounting
- Document Automation
---
