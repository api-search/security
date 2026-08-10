---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vertosmed.com
  spf: true
hosts:
- cert_expires: Mar 10 16:51:06 2027 GMT
  host: www.vertosmed.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vertos Medical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vertos Medical, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vertos Medical
provider_slug: vertos-medical
slug: vertos-medical-domain-security
source_filename: vertos-medical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vertosmed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 10 16:51:06 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: vertosmed.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vertos-medical/refs/heads/main/security/vertos-medical-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Medical Devices
- Health Care
- Spine
- Interventional Pain Management
- Minimally Invasive Surgery
- Acquired
---
