---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: steem.io
  spf: true
hosts:
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: developers.steem.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Steem Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Steem, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Steem
provider_slug: steem
slug: steem-domain-security
source_filename: steem-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.steem.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: steem.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/steem/refs/heads/main/security/steem-domain-security.yml
summary_line: TLSv1.3
tags:
- Blockchain
- Public APIs
---
