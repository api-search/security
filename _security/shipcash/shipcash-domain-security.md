---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: shipcash.net
  spf: true
hosts:
- cert_expires: Sep 23 03:16:41 2026 GMT
  host: shipcash.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shipcash Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ShipCash, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: ShipCash
provider_slug: shipcash
slug: shipcash-domain-security
source_filename: shipcash-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shipcash.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 03:16:41 2026 GMT\n  hsts: null\ndomains:\n- domain: shipcash.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shipcash/refs/heads/main/security/shipcash-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
