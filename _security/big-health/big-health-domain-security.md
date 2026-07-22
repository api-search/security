---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bighealth.com
  spf: true
hosts:
- cert_expires: Sep 28 21:33:31 2026 GMT
  host: bighealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Big Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Big Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Big Health
provider_slug: big-health
slug: big-health-domain-security
source_filename: big-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bighealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 21:33:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bighealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/big-health/refs/heads/main/security/big-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Mental Health
- Digital Therapeutics
- Digital Health
- Behavioral Health
- Wellness
---
