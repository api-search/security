---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: leapstack.tech
  spf: true
hosts:
- cert_expires: Nov 15 11:46:13 2026 GMT
  host: www.leapstack.tech
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Leapstack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LeapStack, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LeapStack
provider_slug: leapstack
slug: leapstack-domain-security
source_filename: leapstack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.leapstack.tech\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 15 11:46:13 2026 GMT\n  hsts: false\ndomains:\n- domain: leapstack.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leapstack/refs/heads/main/security/leapstack-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Fintech
- InsurTech
- Insurance
- Health Insurance
- Data Analytics
- Risk Management
- China
---
