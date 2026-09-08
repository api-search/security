---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: adordx.com
  spf: true
hosts:
- cert_expires: Dec  6 07:52:20 2026 GMT
  host: www.adordx.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Adordiagnostics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ADOR Diagnostics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: ADOR Diagnostics
provider_slug: adordiagnostics
slug: adordiagnostics-domain-security
source_filename: adordiagnostics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.adordx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 07:52:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: adordx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adordiagnostics/refs/heads/main/security/adordiagnostics-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Healthcare
- Medical Devices
- In Vitro Diagnostics
- Molecular Diagnostics
- Infectious Disease
- Point of Care
- Laboratory
- Life Sciences
- MCP
---
