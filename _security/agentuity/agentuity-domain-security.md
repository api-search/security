---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: agentuity.com
  spf: true
hosts:
- cert_expires: Sep  3 00:15:57 2026 GMT
  host: www.agentuity.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agentuity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agentuity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Agentuity
provider_slug: agentuity
slug: agentuity-domain-security
source_filename: agentuity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.agentuity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 00:15:57 2026 GMT\n  hsts: false\ndomains:\n- domain: agentuity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentuity/refs/heads/main/security/agentuity-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Agents
- Artificial Intelligence
- Cloud
- Serverless
- Platform
- Developer Tools
- LLM
- Infrastructure
- Deployment
- AI Gateway
---
