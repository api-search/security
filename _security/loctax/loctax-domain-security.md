---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: loc.tax
  spf: true
hosts:
- cert_expires: Sep 10 18:54:44 2026 GMT
  host: www.loc.tax
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Loctax Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Loctax, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Loctax
provider_slug: loctax
slug: loctax-domain-security
source_filename: loctax-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.loc.tax\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 18:54:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: loc.tax\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loctax/refs/heads/main/security/loctax-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Tax
- Tax Compliance
- Governance
- Risk Management
- Legal Tech
- SaaS
- Fintech
---
