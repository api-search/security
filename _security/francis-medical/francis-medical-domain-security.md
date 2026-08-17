---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: francismedical.com
  spf: true
hosts:
- cert_expires: Nov  9 23:05:28 2026 GMT
  host: www.francismedical.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Francis Medical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Francis Medical, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Francis Medical
provider_slug: francis-medical
slug: francis-medical-domain-security
source_filename: francis-medical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.francismedical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 23:05:28 2026 GMT\n  hsts: false\ndomains:\n- domain: francismedical.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/francis-medical/refs/heads/main/security/francis-medical-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Health Care
- Medical Devices
- Oncology
- Urology
- Prostate Cancer
- Surgery
- Ablation
- Clinical Trials
- Minimally Invasive
---
