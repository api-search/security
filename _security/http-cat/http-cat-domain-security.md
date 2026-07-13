---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: http.cat
  spf: false
hosts:
- cert_expires: Aug 23 02:28:53 2026 GMT
  host: http.cat
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Http Cat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HTTP Cat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: HTTP Cat
provider_slug: http-cat
slug: http-cat-domain-security
source_filename: http-cat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: http.cat\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 02:28:53 2026 GMT\n  hsts: false\ndomains:\n- domain: http.cat\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/http-cat/refs/heads/main/security/http-cat-domain-security.yml
summary_line: TLSv1.3
tags:
- Animals
- Public APIs
---
