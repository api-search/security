---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fundable.com
  spf: true
hosts:
- cert_expires: Dec 29 23:59:59 2026 GMT
  host: www.fundable.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Fundable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fundable, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fundable
provider_slug: fundable
slug: fundable-domain-security
source_filename: fundable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fundable.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 29 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: fundable.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fundable/refs/heads/main/security/fundable-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Fundraising
- Startups
- Crowdfunding
- Investors
- Fintech
- SaaS
---
