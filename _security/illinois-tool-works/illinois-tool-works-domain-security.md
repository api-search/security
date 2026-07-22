---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: itw.com
  spf: true
hosts:
- cert_expires: Jan 23 14:32:24 2027 GMT
  host: www.itw.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Illinois Tool Works Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Illinois Tool Works, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Illinois Tool Works
provider_slug: illinois-tool-works
slug: illinois-tool-works-domain-security
source_filename: illinois-tool-works-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.itw.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 23 14:32:24 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: itw.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/illinois-tool-works/refs/heads/main/security/illinois-tool-works-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Automotive
- Construction
- Fortune 500
- Industrial
- Manufacturing
- Welding
---
