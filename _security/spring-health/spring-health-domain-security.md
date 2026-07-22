---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: springhealth.com
  spf: true
hosts:
- cert_expires: Sep 29 02:42:36 2026 GMT
  host: www.springhealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spring Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spring Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Spring Health
provider_slug: spring-health
slug: spring-health-domain-security
source_filename: spring-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.springhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 02:42:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: springhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spring-health/refs/heads/main/security/spring-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Mental Health
- Behavioral Health
- Employee Benefits
- Employee Assistance Program
- EAP
- Health Plans
- Healthcare
- Therapy
- Medication Management
- Coaching
- Care Navigation
- Digital Health
- Wellbeing
- Workforce Health
- Generative AI
---
