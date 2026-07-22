---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: chmtch.com
  spf: true
hosts:
- cert_expires: Aug 30 03:14:02 2026 GMT
  host: chmtch.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chemtech Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ChemTech AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ChemTech AI
provider_slug: chemtech-ai
slug: chemtech-ai-domain-security
source_filename: chemtech-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chmtch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 03:14:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: chmtch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chemtech-ai/refs/heads/main/security/chemtech-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Industrial Automation
- Chemical Manufacturing
- Process Optimization
- Autonomous Control
- Manufacturing
---
