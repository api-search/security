---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: xapihub.io
  spf: true
hosts:
- cert_expires: Feb 26 23:59:59 2027 GMT
  host: xapihub.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Xapihub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for X-Venture, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: X-Venture
provider_slug: xapihub
slug: xapihub-domain-security
source_filename: xapihub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xapihub.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 26 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: xapihub.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/xapihub/security/xapihub-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Platform
- Marketplace
- Developers
---
