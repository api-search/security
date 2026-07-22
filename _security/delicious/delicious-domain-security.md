---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: delicious.com
  spf: true
hosts:
- cert_expires: Oct 12 12:08:12 2026 GMT
  host: delicious.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Delicious Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Delicious, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Delicious
provider_slug: delicious
slug: delicious-domain-security
source_filename: delicious-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: delicious.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 12:08:12 2026 GMT\n  hsts: false\ndomains:\n- domain: delicious.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/delicious/refs/heads/main/security/delicious-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
---
