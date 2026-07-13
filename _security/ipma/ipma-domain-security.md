---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ipma.pt
  spf: true
hosts:
- cert_expires: Nov 24 10:03:42 2026 GMT
  host: api.ipma.pt
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ipma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IPMA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: IPMA
provider_slug: ipma
slug: ipma-domain-security
source_filename: ipma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.ipma.pt\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 24 10:03:42 2026 GMT\n  hsts: false\ndomains:\n- domain: ipma.pt\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ipma/refs/heads/main/security/ipma-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Weather
- Public APIs
---
