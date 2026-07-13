---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: functionize.com
  spf: true
hosts:
- cert_expires: Sep 23 11:18:49 2026 GMT
  host: www.functionize.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 23:44:07 2026 GMT
  host: support.functionize.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 16:19:17 2026 GMT
  host: app.functionize.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Functionize Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Functionize, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Functionize
provider_slug: functionize
slug: functionize-domain-security
source_filename: functionize-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.functionize.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 11:18:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: support.functionize.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 23:44:07 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n- host: app.functionize.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 16:19:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: functionize.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/functionize/refs/heads/main/security/functionize-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Testing
- Test Automation
- AI Testing
- Generative AI
- QA
- End-to-End Testing
---
