---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: decent.com
  spf: true
hosts:
- cert_expires: Oct 14 09:23:27 2026 GMT
  host: decent.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Decent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Decent, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Decent
provider_slug: decent
slug: decent-domain-security
source_filename: decent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: decent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 09:23:27 2026 GMT\n  hsts: null\ndomains:\n- domain: decent.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/decent/refs/heads/main/security/decent-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
