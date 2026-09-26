---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: atmobiosciences.com
  spf: true
hosts:
- cert_expires: Nov  5 11:37:01 2026 GMT
  host: www.atmobiosciences.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Atmobiosciences Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atmobiosciences, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Atmobiosciences
provider_slug: atmobiosciences
slug: atmobiosciences-domain-security
source_filename: atmobiosciences-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.atmobiosciences.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 11:37:01 2026 GMT\n  hsts: false\ndomains:\n- domain: atmobiosciences.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atmobiosciences/refs/heads/main/security/atmobiosciences-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Bioscience
- Medical Devices
- Gastroenterology
- Diagnostics
- Data Analytics
---
