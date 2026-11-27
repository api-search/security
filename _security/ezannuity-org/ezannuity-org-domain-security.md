---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ezannuity.org
  spf: true
hosts:
- cert_expires: Feb  1 05:12:23 2027 GMT
  host: ezannuity.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: EZ Annuity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EZ Annuity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: EZ Annuity
provider_slug: ezannuity-org
slug: ezannuity-org-domain-security
source_filename: ezannuity-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ezannuity.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 05:12:23 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ezannuity.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/ezannuity-org/security/ezannuity-org-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Finance
- Annuities
- Structured Settlements
- Financial Services
- EZ Annuity
---
