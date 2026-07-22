---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: slan-health.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: vongihealth.com
  spf: true
hosts:
- cert_expires: Feb  9 01:34:41 2027 GMT
  host: www.slan-health.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- host: www.vongihealth.com
  https: false
kind: domain-security
layout: security
method: probed
name: Vongihealth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vongi Health (芝兰健康), probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Vongi Health (芝兰健康)
provider_slug: vongihealth
slug: vongihealth-domain-security
source_filename: vongihealth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.slan-health.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  9 01:34:41 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.vongihealth.com\n  https: false\ndomains:\n- domain: slan-health.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: vongihealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vongihealth/refs/heads/main/security/vongihealth-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- Healthcare
- Digital Therapeutics
- Digital Health
- Hepatitis B
- Sleep
- Medical Devices
- China
---
