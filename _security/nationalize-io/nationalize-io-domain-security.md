---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: nationalize.io
  spf: false
hosts:
- cert_expires: Sep 27 14:12:54 2026 GMT
  host: nationalize.io
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Nationalize Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nationalize.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Nationalize.io
provider_slug: nationalize-io
slug: nationalize-io-domain-security
source_filename: nationalize-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nationalize.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 27 14:12:54 2026 GMT\n  hsts: false\ndomains:\n- domain: nationalize.io\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nationalize-io/refs/heads/main/security/nationalize-io-domain-security.yml
summary_line: TLSv1.2 · DNSSEC
tags:
- Development
- Public APIs
---
