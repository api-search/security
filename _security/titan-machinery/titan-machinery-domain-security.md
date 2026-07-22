---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: titanmachinery.com
  spf: true
hosts:
- cert_expires: Aug 12 21:13:43 2026 GMT
  host: www.titanmachinery.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Titan Machinery Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Titan Machinery, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Titan Machinery
provider_slug: titan-machinery
slug: titan-machinery-domain-security
source_filename: titan-machinery-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.titanmachinery.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 21:13:43 2026 GMT\n  hsts: false\ndomains:\n- domain: titanmachinery.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/titan-machinery/refs/heads/main/security/titan-machinery-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Agriculture
- Construction Equipment
- Heavy Equipment
- Equipment Dealer
- Farm Equipment
---
