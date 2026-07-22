---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: lemonlime.ai
  spf: true
hosts:
- cert_expires: Sep 30 03:19:44 2026 GMT
  host: lemonlime.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lemonlime Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LemonLime, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: LemonLime
provider_slug: lemonlime
slug: lemonlime-domain-security
source_filename: lemonlime-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lemonlime.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 03:19:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lemonlime.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lemonlime/refs/heads/main/security/lemonlime-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Knowledge Management
- AI Agents
- Workflow Automation
- Model Context Protocol
- Enterprise Software
- SaaS
- Y Combinator
---
