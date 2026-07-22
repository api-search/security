---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: observe.ai
  spf: true
hosts:
- cert_expires: Nov 10 10:41:12 2026 GMT
  host: observe.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Observe Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Observe.AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Observe.AI
provider_slug: observe-ai
slug: observe-ai-domain-security
source_filename: observe-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: observe.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 10:41:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: observe.ai\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/observe-ai/refs/heads/main/security/observe-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Contact Center
- Conversation Intelligence
- Customer Service
- Artificial Intelligence
- Voice AI
- Agent Assist
- Speech Analytics
- CCaaS
---
