---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bitcambio.com.br
  spf: true
hosts:
- cert_expires: Sep 28 20:09:32 2026 GMT
  host: nova.bitcambio.com.br
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bitcambio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bitcambio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Bitcambio
provider_slug: bitcambio
slug: bitcambio-domain-security
source_filename: bitcambio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nova.bitcambio.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 20:09:32 2026 GMT\n  hsts: null\ndomains:\n- domain: bitcambio.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitcambio/refs/heads/main/security/bitcambio-domain-security.yml
summary_line: TLSv1.3
tags:
- Cryptocurrency
- Public APIs
---
