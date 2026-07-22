---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: right-hear.com
  spf: true
hosts:
- cert_expires: Mar 20 06:10:58 2027 GMT
  host: right-hear.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Right Hear Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Right Hear, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Right Hear
provider_slug: right-hear
slug: right-hear-domain-security
source_filename: right-hear-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: right-hear.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 20 06:10:58 2027 GMT\n  hsts: false\ndomains:\n- domain: right-hear.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/right-hear/refs/heads/main/security/right-hear-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Accessibility
- Assistive Technology
- Indoor Navigation
- Wayfinding
- Location
- Mobile
- Techstars
---
