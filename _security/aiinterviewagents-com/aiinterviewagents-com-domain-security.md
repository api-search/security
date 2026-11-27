---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aiinterviewagents.com
  spf: true
hosts:
- cert_expires: Jan 25 22:58:29 2027 GMT
  host: aiinterviewagents.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AI Interview Agents Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AI Interview Agents, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AI Interview Agents
provider_slug: aiinterviewagents-com
slug: aiinterviewagents-com-domain-security
source_filename: aiinterviewagents-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aiinterviewagents.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 22:58:29 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aiinterviewagents.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/aiinterviewagents-com/security/aiinterviewagents-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Interviews
- Recruiter Tools
- Candidate Screening
- Video Interview
---
