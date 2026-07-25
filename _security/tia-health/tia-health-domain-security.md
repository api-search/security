---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tiahealth.com
  spf: true
hosts:
- cert_expires: Oct  1 03:46:45 2026 GMT
  host: tiahealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tia Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tia Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tia Health
provider_slug: tia-health
slug: tia-health-domain-security
source_filename: tia-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tiahealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 03:46:45 2026 GMT\n  hsts: false\ndomains:\n- domain: tiahealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tia-health/refs/heads/main/security/tia-health-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Healthcare
- Canada
- Telehealth
- Virtual Care
- Digital Health
- Primary Care
- Mental Health
- Prescriptions
---
