---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cpohq.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: knoetic.com
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:sendgrid.net include:49487496.spf01.hubspotemail.net ~all
hosts:
- cert_expires: Oct 14 00:39:13 2026 GMT
  host: cpohq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 00:39:13 2026 GMT
  host: knoetic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  redirects_to: https://cpohq.com/
  tls_version: TLSv1.3
- cert_expires: Sep  3 10:43:51 2026 GMT
  host: app.knoetic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 14:42:39 2026 GMT
  host: trust.knoetic.com
  hosted_by: vantatrust.com (CNAME)
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Knoetic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Knoetic, probed live across 4 host(s) and 2 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Knoetic
provider_slug: knoetic
slug: knoetic-domain-security
source_filename: knoetic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts (cpohq.com, knoetic.com, app.knoetic.com, trust.knoetic.com)\nnotes: >-\n  knoetic.com 301-redirects to cpohq.com (brand consolidation to CPOHQ); the customer application\n  remains on app.knoetic.com and the trust center on trust.knoetic.com, so both registrable domains\n  are probed.\nhosts:\n- host: cpohq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 00:39:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: knoetic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 00:39:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  redirects_to: https://cpohq.com/\n- host: app.knoetic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 10:43:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: trust.knoetic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 14:42:39 2026 GMT\n  hsts: true\n  hsts_max_age:\
  \ 31536000\n  hsts_include_subdomains: true\n  hosted_by: vantatrust.com (CNAME)\ndomains:\n- domain: cpohq.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n- domain: knoetic.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:_spf.google.com include:sendgrid.net include:49487496.spf01.hubspotemail.net ~all\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/knoetic/refs/heads/main/security/knoetic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Hr Tech
- People Analytics
- Human Resources
- Workforce Analytics
- Artificial Intelligence
- AI Agents
- SaaS
- Community
- Benchmarking
---
