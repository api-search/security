---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: inkblottherapy.com
  spf: true
hosts:
- cert_expires: Sep 13 17:13:50 2026 GMT
  host: inkblottherapy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Inkblot Therapy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Inkblot Therapy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Inkblot Therapy
provider_slug: inkblot-therapy
slug: inkblot-therapy-domain-security
source_filename: inkblot-therapy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: inkblottherapy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 17:13:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: inkblottherapy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inkblot-therapy/refs/heads/main/security/inkblot-therapy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Mental Health
- Healthcare
- Telehealth
- Therapy
- Digital Health
- Employee Assistance Program
- Wellness
---
