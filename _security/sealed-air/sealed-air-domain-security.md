---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: sealed-air.com
  spf: true
hosts:
- cert_expires: Aug 18 23:59:59 2026 GMT
  host: www.sealed-air.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sealed Air Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for sealed-air, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: sealed-air
provider_slug: sealed-air
slug: sealed-air-domain-security
source_filename: sealed-air-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sealed-air.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: sealed-air.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sealed-air/refs/heads/main/security/sealed-air-domain-security.yml
summary_line: TLSv1.3
tags:
- Fortune 500
---
