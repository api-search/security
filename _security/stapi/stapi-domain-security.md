---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: stapi.co
  spf: true
hosts:
- cert_expires: Aug 30 11:03:00 2026 GMT
  host: stapi.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for STAPI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: STAPI
provider_slug: stapi
slug: stapi-domain-security
source_filename: stapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stapi.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 11:03:00 2026 GMT\n  hsts: false\ndomains:\n- domain: stapi.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stapi/refs/heads/main/security/stapi-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Video
- Public APIs
---
