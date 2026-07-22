---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: expertintelligence.ai
  spf: true
hosts:
- cert_expires: Sep  5 22:12:16 2026 GMT
  host: expertintelligence.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Expert Intelligence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Expert Intelligence, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Expert Intelligence
provider_slug: expert-intelligence
slug: expert-intelligence-domain-security
source_filename: expert-intelligence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: expertintelligence.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 22:12:16 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: expertintelligence.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/expert-intelligence/refs/heads/main/security/expert-intelligence-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Pharmaceutical
- Laboratory Automation
- Analytical Chemistry
- Life Sciences
- Data Analytics
- LIMS
---
