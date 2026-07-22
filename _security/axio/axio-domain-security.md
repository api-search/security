---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: axiobio.com
  spf: true
hosts:
- cert_expires: Aug 28 20:37:24 2026 GMT
  host: www.axiobio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Axio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Axio Biosolutions, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Axio Biosolutions
provider_slug: axio
slug: axio-domain-security
source_filename: axio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.axiobio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 20:37:24 2026 GMT\n  hsts: false\ndomains:\n- domain: axiobio.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axio/refs/heads/main/security/axio-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Manufacturing
- Medical Devices
- MedTech
- Healthcare
- Wound Care
- Hemostatic Dressings
- Trauma Care
---
