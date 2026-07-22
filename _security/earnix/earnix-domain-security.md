---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: earnix.com
  spf: true
hosts:
- cert_expires: Sep 27 11:29:55 2026 GMT
  host: earnix.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Earnix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Earnix, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Earnix
provider_slug: earnix
slug: earnix-domain-security
source_filename: earnix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: earnix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 11:29:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: earnix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/earnix/refs/heads/main/security/earnix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Insurance
- InsurTech
- Pricing
- Rating
- Underwriting
- Banking
- Financial Services
- Decisioning
- Artificial Intelligence
---
