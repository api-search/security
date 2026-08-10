---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: axial.net
  spf: true
hosts:
- cert_expires: Sep 24 14:39:14 2026 GMT
  host: www.axial.net
  hsts: true
  hsts_max_age: 604800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Axial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Axial Networks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Axial Networks
provider_slug: axial
slug: axial-domain-security
source_filename: axial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.axial.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 14:39:14 2026 GMT\n  hsts: true\n  hsts_max_age: 604800\ndomains:\n- domain: axial.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axial/refs/heads/main/security/axial-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Mergers and Acquisitions
- Private Capital
- Deal Sourcing
- Financial Services
- Middle Market
- Investment Banking
- Marketplace
---
