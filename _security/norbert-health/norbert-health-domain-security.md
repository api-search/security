---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: norberthealth.com
  spf: true
hosts:
- cert_expires: Nov  8 14:00:00 2026 GMT
  host: www.norberthealth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Norbert Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Norbert Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Norbert Health
provider_slug: norbert-health
slug: norbert-health-domain-security
source_filename: norbert-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.norberthealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 14:00:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: norberthealth.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/norbert-health/refs/heads/main/security/norbert-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Healthtech
- Health
- Remote Patient Monitoring
- Medical Devices
- Robotics
- Artificial Intelligence
- Senior Care
- Vital Signs
- Clinical Documentation
---
