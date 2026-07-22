---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: themis.com
  spf: true
hosts:
- cert_expires: Oct 16 11:56:01 2026 GMT
  host: themis.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Themis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Themis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Themis
provider_slug: themis
slug: themis-domain-security
source_filename: themis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: themis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 11:56:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: themis.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/themis/refs/heads/main/security/themis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Compliance
- Governance Risk Compliance
- Risk Management
- Vendor Management
- Audit
- Fintech
- Banking
- Regulatory Technology
---
