---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fairlyne.com
  spf: true
hosts:
- cert_expires: Sep 22 07:51:30 2026 GMT
  host: www.fairlyne.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fairlyne Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fairlyne, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fairlyne
provider_slug: fairlyne
slug: fairlyne-domain-security
source_filename: fairlyne-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fairlyne.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 07:51:30 2026 GMT\n  hsts: false\ndomains:\n- domain: fairlyne.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fairlyne/refs/heads/main/security/fairlyne-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Travel
- Travel Technology
- SaaS
- Resale
- Airlines
- Rail
- Hospitality
---
