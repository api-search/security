---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: innertrends.com
  spf: false
hosts:
- cert_expires: Sep  2 23:14:01 2026 GMT
  host: innertrends.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Innertrends Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Innertrends, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Innertrends
provider_slug: innertrends
slug: innertrends-domain-security
source_filename: innertrends-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: innertrends.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 23:14:01 2026 GMT\n  hsts: false\ndomains:\n- domain: innertrends.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/innertrends/refs/heads/main/security/innertrends-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Analytics
- Product Analytics
- Marketing
- Growth
- Data
- SaaS
- Consulting
- Attribution
---
