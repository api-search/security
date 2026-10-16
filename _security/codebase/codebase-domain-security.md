---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: codebase.com
  spf: true
hosts:
- cert_expires: Nov 30 02:43:03 2026 GMT
  host: www.codebase.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Codebase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Codebase, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Codebase
provider_slug: codebase
slug: codebase-domain-security
source_filename: codebase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.codebase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 02:43:03 2026 GMT\n  hsts: false\ndomains:\n- domain: codebase.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codebase/refs/heads/main/security/codebase-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Software Development
- Offshore Teams
- Agile
- Digital Products
---
