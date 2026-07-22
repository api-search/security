---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: journeyclinical.com
  spf: true
hosts:
- cert_expires: Aug 28 05:17:48 2026 GMT
  host: www.journeyclinical.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Journey Clinical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Journey Clinical, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Journey Clinical
provider_slug: journey-clinical
slug: journey-clinical-domain-security
source_filename: journey-clinical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.journeyclinical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 05:17:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: journeyclinical.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/journey-clinical/refs/heads/main/security/journey-clinical-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Telehealth
- Mental Health
- Healthcare
- Ketamine-Assisted Psychotherapy
- Medication Management
- HIPAA
- Digital Health
---
