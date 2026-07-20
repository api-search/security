---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mammothcyber.com
  spf: true
hosts:
- cert_expires: Aug 24 21:08:03 2026 GMT
  host: mammothcyber.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Appaegis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Appaegis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Appaegis
provider_slug: appaegis
slug: appaegis-domain-security
source_filename: appaegis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mammothcyber.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 21:08:03 2026 GMT\n  hsts: false\ndomains:\n- domain: mammothcyber.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appaegis/refs/heads/main/security/appaegis-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Security
- Zero Trust
- Enterprise Browser
- Access Management
- Data Loss Prevention
- GenAI Security
- Identity
- SASE
---
