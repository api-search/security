---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fincompare.de
  spf: true
hosts:
- cert_expires: Oct 10 03:35:24 2026 GMT
  host: fincompare.de
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fincompare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fincompare, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fincompare
provider_slug: fincompare
slug: fincompare-domain-security
source_filename: fincompare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fincompare.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 03:35:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fincompare.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fincompare/refs/heads/main/security/fincompare-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financing
- SME Lending
- Fintech
- Loans
- Comparison Marketplace
- Banking
- Factoring
- Leasing
- Germany
---
