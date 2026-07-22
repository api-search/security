---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: swiftmedical.com
  spf: true
hosts:
- cert_expires: Sep 13 18:31:45 2026 GMT
  host: swiftmedical.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Swift Medical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Swift Medical, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Swift Medical
provider_slug: swift-medical
slug: swift-medical-domain-security
source_filename: swift-medical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: swiftmedical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 18:31:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: swiftmedical.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swift-medical/refs/heads/main/security/swift-medical-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Healthcare
- Wound Care
- Medical Imaging
- Artificial Intelligence
- Digital Health
- Clinical Software
---
