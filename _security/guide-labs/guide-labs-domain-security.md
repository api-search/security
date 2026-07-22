---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: guidelabs.ai
  spf: true
hosts:
- cert_expires: Oct  6 10:44:35 2026 GMT
  host: www.guidelabs.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Guide Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Guide Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Guide Labs
provider_slug: guide-labs
slug: guide-labs-domain-security
source_filename: guide-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.guidelabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 10:44:35 2026 GMT\n  hsts: false\ndomains:\n- domain: guidelabs.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/guide-labs/refs/heads/main/security/guide-labs-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Enterprise Saas
- Artificial Intelligence
- Interpretability
- Machine Learning
- Foundation Models
- Large Language Models
- AI Safety
- Research
---
