---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: blinkidentity.com
  spf: true
hosts:
- cert_expires: Aug 22 01:10:24 2026 GMT
  host: blinkidentity.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blink Identity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blink Identity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Blink Identity
provider_slug: blink-identity
slug: blink-identity-domain-security
source_filename: blink-identity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blinkidentity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 01:10:24 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: blinkidentity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blink-identity/refs/heads/main/security/blink-identity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Identity
- Biometrics
- Facial Recognition
- Authentication
- Live Events
- Ticketing
- Payments
- Privacy
---
