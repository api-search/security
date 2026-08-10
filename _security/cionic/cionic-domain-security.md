---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cionic.com
  spf: true
hosts:
- cert_expires: Oct 31 09:02:01 2026 GMT
  host: www.cionic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 07:30:49 2026 GMT
  host: cionic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cionic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CIONIC, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CIONIC
provider_slug: cionic
slug: cionic-domain-security
source_filename: cionic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cionic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 09:02:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cionic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 07:30:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cionic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cionic/refs/heads/main/security/cionic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Medical Devices
- Wearables
- Neurotechnology
- Research
- Clinical Research
- Biomechanics
- Rehabilitation
- Digital Health
---
