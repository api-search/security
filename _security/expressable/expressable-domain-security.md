---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: expressable.com
  spf: false
hosts:
- cert_expires: Oct 20 02:45:57 2026 GMT
  host: www.expressable.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Expressable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Expressable, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Expressable
provider_slug: expressable
slug: expressable-domain-security
source_filename: expressable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.expressable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 02:45:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: expressable.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/expressable/refs/heads/main/security/expressable-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Health
- Healthcare
- Telehealth
- Speech Therapy
- Teletherapy
- Digital Health
- Consumer Health
- Behavioral Health
---
