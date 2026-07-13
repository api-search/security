---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: binlist.net
  spf: true
hosts:
- cert_expires: Sep 15 05:09:52 2026 GMT
  host: binlist.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Binlist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Binlist, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Binlist
provider_slug: binlist
slug: binlist-domain-security
source_filename: binlist-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: binlist.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 05:09:52 2026 GMT\n  hsts: false\ndomains:\n- domain: binlist.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/binlist/refs/heads/main/security/binlist-domain-security.yml
summary_line: TLSv1.3
tags:
- Finance
- Public APIs
---
