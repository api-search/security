---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vrmedical.net
  spf: true
hosts:
- cert_expires: Sep 28 07:30:45 2026 GMT
  host: vrmedical.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vrmedical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VR Medical, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: VR Medical
provider_slug: vrmedical
slug: vrmedical-domain-security
source_filename: vrmedical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vrmedical.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 07:30:45 2026 GMT\n  hsts: null\ndomains:\n- domain: vrmedical.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vrmedical/refs/heads/main/security/vrmedical-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Medical Devices
- Healthcare
- Respiratory Care
- Wound Care
- Critical Care
- Manufacturing
---
