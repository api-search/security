---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ai-lifeline.org
  spf: true
hosts:
- cert_expires: Jan 19 16:14:23 2027 GMT
  host: ai-lifeline.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AI Lifeline Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AI Lifeline, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AI Lifeline
provider_slug: ai-lifeline-org
slug: ai-lifeline-org-domain-security
source_filename: ai-lifeline-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ai-lifeline.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 16:14:23 2027 GMT\n  hsts: false\ndomains:\n- domain: ai-lifeline.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ai-lifeline-org/security/ai-lifeline-org-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Observatory
- Data
- Sustainability
- Research
---
