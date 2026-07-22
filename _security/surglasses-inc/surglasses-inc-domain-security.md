---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: surglasses.com
  spf: false
hosts:
- cert_expires: Sep  8 10:15:21 2026 GMT
  host: surglasses.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Surglasses Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Surglasses Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Surglasses Inc.
provider_slug: surglasses-inc
slug: surglasses-inc-domain-security
source_filename: surglasses-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: surglasses.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  8 10:15:21 2026 GMT\n  hsts: false\ndomains:\n- domain: surglasses.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/surglasses-inc/refs/heads/main/security/surglasses-inc-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Medical Devices
- Augmented Reality
- Surgical Navigation
- Healthcare
- Medical Education
- Health Tech
---
