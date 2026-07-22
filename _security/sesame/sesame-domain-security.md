---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sesamecare.com
  spf: true
hosts:
- cert_expires: Oct  8 08:57:03 2026 GMT
  host: sesamecare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sesame Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sesame, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sesame
provider_slug: sesame
slug: sesame-domain-security
source_filename: sesame-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sesamecare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 08:57:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sesamecare.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sesame/refs/heads/main/security/sesame-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Telehealth
- Healthcare
- Digital Health
- Telemedicine
- Marketplace
- Consumer Health
- Prescriptions
---
