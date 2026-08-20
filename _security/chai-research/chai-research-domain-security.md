---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: chai-research.com
  spf: true
hosts:
- cert_expires: Sep 19 12:31:32 2026 GMT
  host: www.chai-research.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chai Research Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chai Research, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Chai Research
provider_slug: chai-research
slug: chai-research-domain-security
source_filename: chai-research-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chai-research.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 12:31:32 2026 GMT\n  hsts: false\ndomains:\n- domain: chai-research.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chai-research/refs/heads/main/security/chai-research-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Large Language Models
- Conversational AI
- Chatbots
- Consumer Applications
- Machine-Learning
- Model Hosting
---
