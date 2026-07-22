---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: homeday.de
  spf: true
hosts:
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: homeday.de
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Homeday Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Homeday, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Homeday
provider_slug: homeday
slug: homeday-domain-security
source_filename: homeday-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: homeday.de\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: homeday.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/homeday/refs/heads/main/security/homeday-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Real Estate
- PropTech
- Germany
- Brokerage
- Mortgage
- Property Valuation
---
