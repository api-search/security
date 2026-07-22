---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cadee.co
  spf: true
hosts:
- cert_expires: Sep 23 03:25:56 2026 GMT
  host: cadee.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cadee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cadee, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Cadee
provider_slug: cadee
slug: cadee-domain-security
source_filename: cadee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cadee.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 03:25:56 2026 GMT\n  hsts: null\ndomains:\n- domain: cadee.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cadee/refs/heads/main/security/cadee-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
