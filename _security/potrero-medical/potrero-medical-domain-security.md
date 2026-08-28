---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: accuryn.com
  spf: true
hosts:
- cert_expires: Nov  1 01:43:52 2026 GMT
  host: accuryn.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Potrero Medical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Potrero Medical, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Potrero Medical
provider_slug: potrero-medical
slug: potrero-medical-domain-security
source_filename: potrero-medical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: accuryn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 01:43:52 2026 GMT\n  hsts: false\ndomains:\n- domain: accuryn.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/potrero-medical/refs/heads/main/security/potrero-medical-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Medical Devices
- Healthcare
- Patient Monitoring
- Critical Care
- Medical Device Integration
- Predictive Health
---
