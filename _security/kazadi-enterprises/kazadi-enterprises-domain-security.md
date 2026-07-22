---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kazadienterprises.com
  spf: true
hosts:
- cert_expires: Sep  6 18:30:30 2026 GMT
  host: kazadienterprises.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kazadi Enterprises Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kazadi Enterprises, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kazadi Enterprises
provider_slug: kazadi-enterprises
slug: kazadi-enterprises-domain-security
source_filename: kazadi-enterprises-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kazadienterprises.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 18:30:30 2026 GMT\n  hsts: null\ndomains:\n- domain: kazadienterprises.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kazadi-enterprises/refs/heads/main/security/kazadi-enterprises-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Renewable Energy
- Cold Chain
- Dehumidification
- Climate Control
- Controlled Environment Agriculture
- Cleantech
---
