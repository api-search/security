---
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "amazon.com"
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: 1mind.com
  spf: true
hosts:
- cert_expires: Sep 30 09:20:47 2026 GMT
  host: www.1mind.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 1Mind Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 1mind AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: 1mind AI
provider_slug: 1mind-ai
slug: 1mind-ai-domain-security
source_filename: 1mind-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.1mind.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 09:20:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: 1mind.com\n  dnssec: true\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1mind-ai/refs/heads/main/security/1mind-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Sales
- Go-To-Market
- AI Agents
- Conversational AI
- Revenue Operations
---
