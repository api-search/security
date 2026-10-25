---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gendevelopmentgroup.com.au
  spf: true
hosts:
- cert_expires: Dec 22 12:02:30 2026 GMT
  host: gendevelopmentgroup.com.au
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Generation Development Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Generation Development Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Generation Development Group
provider_slug: generation-development-group
slug: generation-development-group-domain-security
source_filename: generation-development-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gendevelopmentgroup.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 12:02:30 2026 GMT\n  hsts: false\ndomains:\n- domain: gendevelopmentgroup.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/generation-development-group/refs/heads/main/security/generation-development-group-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Financial Services
- Investment Bonds
- Annuities
- Managed Accounts
- Investment Research
- Australia
- ASX Listed
---
