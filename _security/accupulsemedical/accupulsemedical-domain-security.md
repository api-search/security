---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: accupulse.com
  spf: true
hosts:
- cert_expires: Oct  8 01:59:59 2026 GMT
  host: accupulse.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Accupulsemedical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AccuPulse Medical Technology Co., Ltd., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AccuPulse Medical Technology Co., Ltd.
provider_slug: accupulsemedical
slug: accupulsemedical-domain-security
source_filename: accupulsemedical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: accupulse.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  8 01:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: accupulse.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accupulsemedical/refs/heads/main/security/accupulsemedical-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Medical Devices
- Health Care
- Cardiology
- Electrophysiology
- Cardiac Ablation
- Medical Imaging
- Manufacturing
- China
---
