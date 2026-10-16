---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: contegomedical.com
  spf: true
hosts:
- cert_expires: Nov 29 05:48:23 2026 GMT
  host: contegomedical.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Contego Medical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Contego Medical, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Contego Medical
provider_slug: contego-medical
slug: contego-medical-domain-security
source_filename: contego-medical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: contegomedical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 05:48:23 2026 GMT\n  hsts: null\ndomains:\n- domain: contegomedical.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contego-medical/refs/heads/main/security/contego-medical-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Medical Devices
- Vascular
- Revascularization
- Embolic Protection
- Healthcare
---
