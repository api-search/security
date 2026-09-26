---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: arsenalmedical.com
  spf: true
hosts:
- cert_expires: Dec 13 10:49:36 2026 GMT
  host: arsenalmedical.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Arsenal Medical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arsenal Medical, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Arsenal Medical
provider_slug: arsenal-medical
slug: arsenal-medical-domain-security
source_filename: arsenal-medical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arsenalmedical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 10:49:36 2026 GMT\n  hsts: false\ndomains:\n- domain: arsenalmedical.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arsenal-medical/refs/heads/main/security/arsenal-medical-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Medical Devices
- Biomaterials
- Healthcare
- Innovation
- Company
---
