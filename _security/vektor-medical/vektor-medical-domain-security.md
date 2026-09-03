---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vektormedical.com
  spf: true
hosts:
- cert_expires: Oct 12 11:14:16 2026 GMT
  host: www.vektormedical.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vektor Medical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vektor Medical, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vektor Medical
provider_slug: vektor-medical
slug: vektor-medical-domain-security
source_filename: vektor-medical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vektormedical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 11:14:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vektormedical.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vektor-medical/refs/heads/main/security/vektor-medical-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Medical Devices
- Healthcare
- Cardiology
- Electrophysiology
- Artificial Intelligence
- Software as a Medical Device
- Diagnostics
---
