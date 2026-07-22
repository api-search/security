---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lilium.com
  spf: true
hosts:
- host: lilium.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Lilium Air Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lilium, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lilium
provider_slug: lilium-air
slug: lilium-air-domain-security
source_filename: lilium-air-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lilium.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: lilium.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lilium-air/refs/heads/main/security/lilium-air-domain-security.yml
summary_line: DMARC
tags:
- Advanced Air Mobility
- Aerospace
- Air Taxi
- Defunct
- eVTOL
- EASA Certification
- Electric Aviation
- Germany
- Insolvency
- Regional Air Mobility
---
