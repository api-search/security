---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: interviewflowai.com
  spf: true
hosts:
- cert_expires: Feb  6 07:11:13 2027 GMT
  host: interviewflowai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: InterviewFlowAI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for InterviewFlowAI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: InterviewFlowAI
provider_slug: interviewflowai-com
slug: interviewflowai-com-domain-security
source_filename: interviewflowai-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: interviewflowai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 07:11:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: interviewflowai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/interviewflowai-com/security/interviewflowai-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Hiring
- Interview
- Automation
- Software-as-a-Service
---
