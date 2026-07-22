---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: welltower.com
  spf: true
hosts:
- cert_expires: Oct  6 23:31:55 2026 GMT
  host: welltower.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Welltower Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for welltower, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: welltower
provider_slug: welltower
slug: welltower-domain-security
source_filename: welltower-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: welltower.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:31:55 2026 GMT\n  hsts: false\ndomains:\n- domain: welltower.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/welltower/refs/heads/main/security/welltower-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Fortune 1000
---
