---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cixtech.com
  spf: true
hosts:
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: cixtech.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cixtech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CIX Technology, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: CIX Technology
provider_slug: cixtech
slug: cixtech-domain-security
source_filename: cixtech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cixtech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: cixtech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cixtech/refs/heads/main/security/cixtech-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Semiconductors
- CPU
- Artificial Intelligence
- Edge Computing
- Automotive
- Hardware
- Arm
---
