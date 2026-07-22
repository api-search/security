---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gilt.com
  spf: true
hosts:
- cert_expires: Feb 22 23:59:59 2027 GMT
  host: www.gilt.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gilt Groupe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gilt Groupe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Gilt Groupe
provider_slug: gilt-groupe
slug: gilt-groupe-domain-security
source_filename: gilt-groupe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gilt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 22 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: gilt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gilt-groupe/refs/heads/main/security/gilt-groupe-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Retail
- E-commerce
- Fashion
- Flash Sale
- Scala
- Open Source
---
