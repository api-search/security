---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: chatterresearch.com
  spf: true
hosts:
- cert_expires: Sep 25 23:08:46 2026 GMT
  host: chatterresearch.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chatter Research Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chatter Research, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Chatter Research
provider_slug: chatter-research
slug: chatter-research-domain-security
source_filename: chatter-research-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chatterresearch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:08:46 2026 GMT\n  hsts: false\ndomains:\n- domain: chatterresearch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chatter-research/refs/heads/main/security/chatter-research-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Customer Feedback
- Customer Experience
- Surveys
- Voice of Customer
- Retail
- NPS
- Sentiment Analysis
---
