---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mybrightwheel.com
  spf: true
hosts:
- cert_expires: Mar  7 23:59:59 2027 GMT
  host: mybrightwheel.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brightwheel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brightwheel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Brightwheel
provider_slug: brightwheel
slug: brightwheel-domain-security
source_filename: brightwheel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mybrightwheel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  7 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: mybrightwheel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brightwheel/refs/heads/main/security/brightwheel-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Childcare
- Early Education
- Preschool
- Childcare Management
- Attendance
- Billing
- Payments
- Parent Communication
- EdTech
- No Public API
---
