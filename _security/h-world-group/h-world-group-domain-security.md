---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hworld.com
  spf: true
hosts:
- cert_expires: Aug 24 23:59:59 2026 GMT
  host: www.hworld.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: H World Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for H World Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: H World Group
provider_slug: h-world-group
slug: h-world-group-domain-security
source_filename: h-world-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hworld.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: hworld.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/h-world-group/refs/heads/main/security/h-world-group-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Consumer
- Hotels
- Hospitality
- Travel
- Lodging
- China
- Loyalty
---
