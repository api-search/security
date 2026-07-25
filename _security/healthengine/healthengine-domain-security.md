---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: healthengine.com.au
  spf: true
hosts:
- cert_expires: Mar 13 23:59:59 2027 GMT
  host: healthengine.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: practices.healthengine.com.au
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Healthengine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HealthEngine, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: HealthEngine
provider_slug: healthengine
slug: healthengine-domain-security
source_filename: healthengine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: healthengine.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 13 23:59:59 2027 GMT\n  hsts: null\n- host: practices.healthengine.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: healthengine.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/healthengine/refs/heads/main/security/healthengine-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Australia
- Patient Engagement
- Appointment Booking
- Scheduling
- Telehealth
- Practice Management
- Digital Health
- Healthcare Marketplace
- Interoperability
---
