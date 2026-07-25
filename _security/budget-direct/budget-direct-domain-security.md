---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: budgetdirect.com.au
  spf: true
hosts:
- cert_expires: Sep 16 15:38:46 2026 GMT
  host: www.budgetdirect.com.au
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Budget Direct Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Budget Direct, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Budget Direct
provider_slug: budget-direct
slug: budget-direct-domain-security
source_filename: budget-direct-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.budgetdirect.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 15:38:46 2026 GMT\n  hsts: false\ndomains:\n- domain: budgetdirect.com.au\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/budget-direct/refs/heads/main/security/budget-direct-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Insurance
- Australia
- Property and Casualty
- Direct to Consumer Insurance
- Motor Insurance
- Home Insurance
- Travel Insurance
- Life Insurance
- Underwriting
- Claims
- Carrier
- No Public API
---
