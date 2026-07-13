---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: onetrust.com
  spf: true
hosts:
- cert_expires: Oct  5 03:46:04 2026 GMT
  host: www.onetrust.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 01:05:41 2026 GMT
  host: developer.onetrust.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tugboat Logic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tugboat Logic, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Tugboat Logic
provider_slug: tugboat-logic
slug: tugboat-logic-domain-security
source_filename: tugboat-logic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.onetrust.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 03:46:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.onetrust.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 01:05:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: onetrust.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tugboat-logic/refs/heads/main/security/tugboat-logic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- GRC
- Compliance
- SOC 2
- ISO 27001
- Security
---
