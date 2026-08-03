---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: capstanmedical.com
  spf: true
hosts:
- cert_expires: Sep 27 10:29:15 2026 GMT
  host: capstanmedical.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Capstan Medical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Capstan Medical, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Capstan Medical
provider_slug: capstan-medical
slug: capstan-medical-domain-security
source_filename: capstan-medical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: capstanmedical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 10:29:15 2026 GMT\n  hsts: false\ndomains:\n- domain: capstanmedical.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capstan-medical/refs/heads/main/security/capstan-medical-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Medical Devices
- Surgical Robotics
- Structural Heart
- Cardiovascular
- Healthcare
- Robotics
- Medical Technology
---
