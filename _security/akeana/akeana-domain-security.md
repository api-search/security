---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: akeana.com
  spf: true
hosts:
- cert_expires: Oct  9 05:28:33 2026 GMT
  host: akeana.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Akeana Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Akeana, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Akeana
provider_slug: akeana
slug: akeana-domain-security
source_filename: akeana-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: akeana.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 05:28:33 2026 GMT\n  hsts: false\ndomains:\n- domain: akeana.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akeana/refs/heads/main/security/akeana-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Hardtech
- Semiconductors
- RISC-V
- Processors
- Silicon IP
- Artificial Intelligence
---
