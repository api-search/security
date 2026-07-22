---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: joinajax.com
  spf: true
hosts:
- cert_expires: Aug 30 11:07:04 2026 GMT
  host: www.joinajax.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ajax Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ajax, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Ajax
provider_slug: ajax
slug: ajax-domain-security
source_filename: ajax-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.joinajax.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 11:07:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: joinajax.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ajax/refs/heads/main/security/ajax-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Legal
- Legal Tech
- Timekeeping
- Billing
- Law Firms
- AI
- Productivity
- SaaS
---
