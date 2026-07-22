---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: seevividly.com
  spf: true
hosts:
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: www.seevividly.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Vivid Vision Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vivid Vision, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vivid Vision
provider_slug: vivid-vision
slug: vivid-vision-domain-security
source_filename: vivid-vision-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.seevividly.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: seevividly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vivid-vision/refs/heads/main/security/vivid-vision-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Vision Care
- Health
- Virtual Reality
- Ophthalmology
- Vision Therapy
- Clinical Trials
- MedTech
---
