---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: inquismedical.com
  spf: true
hosts:
- cert_expires: Nov 20 23:44:47 2026 GMT
  host: inquismedical.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Inquis Medical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Inquis Medical, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Inquis Medical
provider_slug: inquis-medical
slug: inquis-medical-domain-security
source_filename: inquis-medical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: inquismedical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 23:44:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: inquismedical.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inquis-medical/refs/heads/main/security/inquis-medical-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Medical Devices
- Thrombectomy
- Interventional Radiology
- Cardiovascular
- Pulmonary Embolism
- Catheters
- Clinical Trials
- Medical Hardware
---
