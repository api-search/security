---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: carallel.com
  spf: true
hosts:
- cert_expires: Nov 23 03:48:07 2026 GMT
  host: carallel.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Carallelllc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carallelllc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Carallelllc
provider_slug: carallelllc
slug: carallelllc-domain-security
source_filename: carallelllc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: carallel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 03:48:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: carallel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carallelllc/refs/heads/main/security/carallelllc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Digital Health
- Caregiver Support
- Health Plans
- Providers
- Employers
---
