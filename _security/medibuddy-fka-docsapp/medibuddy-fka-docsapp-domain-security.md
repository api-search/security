---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: medibuddy.in
  spf: true
hosts:
- cert_expires: Jul 31 23:59:59 2026 GMT
  host: www.medibuddy.in
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Medibuddy Fka Docsapp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MediBuddy (fka DocsApp), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MediBuddy (fka DocsApp)
provider_slug: medibuddy-fka-docsapp
slug: medibuddy-fka-docsapp-domain-security
source_filename: medibuddy-fka-docsapp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.medibuddy.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: medibuddy.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medibuddy-fka-docsapp/refs/heads/main/security/medibuddy-fka-docsapp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Telemedicine
- Telehealth
- Doctor Consultation
- Lab Tests
- Online Pharmacy
- Digital Health
- India
---
