---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kangoapp.co
  spf: false
hosts:
- cert_expires: Oct 11 23:59:59 2026 GMT
  host: kangoapp.co
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Kango Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kango, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Kango
provider_slug: kango
slug: kango-domain-security
source_filename: kango-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kangoapp.co\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: kangoapp.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kango/refs/heads/main/security/kango-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Childcare
- Transportation
- Ridesharing
- Family
- Mobility
- On-Demand
---
