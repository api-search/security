---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: theguarantors.com
  spf: true
hosts:
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: theguarantors.com
  hsts: true
  hsts_max_age: 1800
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Theguarantors Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TheGuarantors, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TheGuarantors
provider_slug: theguarantors
slug: theguarantors-domain-security
source_filename: theguarantors-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: theguarantors.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 1800\ndomains:\n- domain: theguarantors.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/theguarantors/refs/heads/main/security/theguarantors-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Financial Services
- Fintech
- Insurance
- Real Estate
- Rental
- PropTech
- Lease Guarantee
- Renters Insurance
- API
---
