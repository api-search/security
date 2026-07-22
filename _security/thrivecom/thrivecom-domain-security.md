---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ringcaptcha.com
  spf: true
hosts:
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: ringcaptcha.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Thrivecom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RingCaptcha (ThriveCom), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: RingCaptcha (ThriveCom)
provider_slug: thrivecom
slug: thrivecom-domain-security
source_filename: thrivecom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ringcaptcha.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ringcaptcha.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thrivecom/refs/heads/main/security/thrivecom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Two-Factor Authentication
- Phone Verification
- One-Time Passcode
- SMS
- Voice
- Fraud Prevention
- Identity Verification
- Authentication
---
