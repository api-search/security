---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: stel.life
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: stelhealth.com
  spf: true
hosts:
- cert_expires: Aug 31 05:06:18 2026 GMT
  host: www.stel.life
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: manage.stelhealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stel, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Stel
provider_slug: stel
slug: stel-domain-security
source_filename: stel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stel.life\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 05:06:18 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: manage.stelhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: stel.life\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: stelhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stel/refs/heads/main/security/stel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Remote Patient Monitoring
- Connected Health
- Medical Devices
- Digital Health
- EHR Integration
- Telehealth
- IoT
---
