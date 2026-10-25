---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: newhopegroup.com.au
  spf: true
hosts:
- cert_expires: Nov 26 00:16:13 2026 GMT
  host: newhopegroup.com.au
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: New Hope Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for New Hope Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: New Hope Group
provider_slug: new-hope
slug: new-hope-domain-security
source_filename: new-hope-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: newhopegroup.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 00:16:13 2026 GMT\n  hsts: false\ndomains:\n- domain: newhopegroup.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/new-hope/refs/heads/main/security/new-hope-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Coal Mining
- Energy
- Agriculture
- Australia
- ASX Listed
- Resources
---
