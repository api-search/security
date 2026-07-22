---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: freeagency.com
  spf: true
hosts:
- cert_expires: Aug 30 01:56:08 2026 GMT
  host: www.freeagency.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Free Agency Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Free Agency, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Free Agency
provider_slug: free-agency
slug: free-agency-domain-security
source_filename: free-agency-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.freeagency.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 01:56:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: freeagency.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/free-agency/refs/heads/main/security/free-agency-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Careers
- Talent
- Recruiting
- Marketplace
- Jobs
- AI
- Newsletter
---
