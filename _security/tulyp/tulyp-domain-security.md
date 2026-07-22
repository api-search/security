---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: tulyp.io
  spf: true
hosts:
- cert_expires: Aug 25 11:33:22 2026 GMT
  host: tulyp.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tulyp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tulyp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Tulyp
provider_slug: tulyp
slug: tulyp-domain-security
source_filename: tulyp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tulyp.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 11:33:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tulyp.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tulyp/refs/heads/main/security/tulyp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- FinTech
- Treasury
- Foreign Exchange
- Risk Management
- SaaS
- France
---
