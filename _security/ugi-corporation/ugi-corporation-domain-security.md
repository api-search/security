---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ugicorp.com
  spf: true
hosts:
- cert_expires: Aug 11 07:06:45 2026 GMT
  host: www.ugicorp.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ugi Corporation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UGI Corporation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: UGI Corporation
provider_slug: ugi-corporation
slug: ugi-corporation-domain-security
source_filename: ugi-corporation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ugicorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 07:06:45 2026 GMT\n  hsts: null\ndomains:\n- domain: ugicorp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ugi-corporation/refs/heads/main/security/ugi-corporation-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Energy
- Utility
- Natural Gas
- Electric
- Propane
- LPG
- Midstream
- Fortune 500
---
