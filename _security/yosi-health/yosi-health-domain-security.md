---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: yosi.health
  spf: false
hosts:
- cert_expires: Dec 24 13:12:22 2026 GMT
  host: yosi.health
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Yosi Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yosi Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Yosi Health
provider_slug: yosi-health
slug: yosi-health-domain-security
source_filename: yosi-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yosi.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 13:12:22 2026 GMT\n  hsts: false\ndomains:\n- domain: yosi.health\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/yosi-health/security/yosi-health-domain-security.yml
summary_line: TLSv1.3
tags:
- Healthcare
- Patient Intake
- Telehealth
- Scheduling
- Payments
---
