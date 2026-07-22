---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: blazemeter.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: runscope.com
  spf: true
hosts:
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: help.blazemeter.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 01:45:32 2026 GMT
  host: api.runscope.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Runscope Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Runscope, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Runscope
provider_slug: runscope
slug: runscope-domain-security
source_filename: runscope-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: help.blazemeter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.runscope.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 01:45:32 2026 GMT\n  hsts: null\ndomains:\n- domain: blazemeter.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: runscope.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/runscope/refs/heads/main/security/runscope-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- API Monitoring
- API Testing
- Observability
- Synthetic Monitoring
- Developer Tools
- Quality Assurance
---
