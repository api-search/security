---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: jane.app
  spf: true
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jane.qa
  spf: false
hosts:
- cert_expires: Sep 11 19:57:27 2026 GMT
  host: jane.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 17:00:41 2026 GMT
  host: developers.jane.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: jdpdocsdemo.jane.qa
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jane App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jane, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Jane
provider_slug: jane-app
slug: jane-app-domain-security
source_filename: jane-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jane.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 19:57:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.jane.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 17:00:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: jdpdocsdemo.jane.qa\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: jane.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: jane.qa\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jane-app/refs/heads/main/security/jane-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Canada
- Practice Management
- EHR
- EMR
- Scheduling
- Clinical Documentation
- Telehealth
- Health and Wellness
- REST API
- OAuth2
- Webhooks
---
