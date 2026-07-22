---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: njresources.com
  spf: true
hosts:
- cert_expires: Feb 17 23:59:59 2027 GMT
  host: www.njresources.com
  hsts: true
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: New Jersey Resources Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for New Jersey Resources, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: New Jersey Resources
provider_slug: new-jersey-resources
slug: new-jersey-resources-domain-security
source_filename: new-jersey-resources-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.njresources.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 17 23:59:59 2027 GMT\n  hsts: true\ndomains:\n- domain: njresources.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/new-jersey-resources/refs/heads/main/security/new-jersey-resources-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Natural Gas
- Utilities
- Clean Energy
- Fortune 1000
---
