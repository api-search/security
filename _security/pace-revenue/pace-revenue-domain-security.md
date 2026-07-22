---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: flyr.com
  spf: true
hosts:
- cert_expires: Sep  9 11:06:21 2026 GMT
  host: flyr.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pace Revenue Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pace Revenue, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Pace Revenue
provider_slug: pace-revenue
slug: pace-revenue-domain-security
source_filename: pace-revenue-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flyr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 11:06:21 2026 GMT\n  hsts: false\ndomains:\n- domain: flyr.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pace-revenue/refs/heads/main/security/pace-revenue-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Hospitality
- Hotels
- Revenue Management
- Dynamic Pricing
- Machine Learning
- Travel
- Pricing
---
