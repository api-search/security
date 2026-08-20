---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cresta.com
  spf: true
hosts:
- cert_expires: Nov  1 20:48:05 2026 GMT
  host: cresta.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 23:59:59 2026 GMT
  host: developers.cresta.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 20:48:05 2026 GMT
  host: api.cresta.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_note: 'The probe script records null here because the gRPC-JSON gateway answers its HEAD with 405. A direct GET on 2026-08-14 returned "strict-transport-security: max-age=31536000; includeSubDomains", so HSTS is present on the API host. Corrected by hand; re-running 0-working/probe-domain-security.py will revert it to null.'
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cresta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cresta, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Cresta
provider_slug: cresta
slug: cresta-domain-security
source_filename: cresta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cresta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 20:48:05 2026 GMT\n  hsts: false\n- host: developers.cresta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 23:59:59 2026 GMT\n  hsts: false\n- host: api.cresta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 20:48:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_note: >-\n    The probe script records null here because the gRPC-JSON gateway answers\n    its HEAD with 405. A direct GET on 2026-08-14 returned\n    \"strict-transport-security: max-age=31536000; includeSubDomains\", so HSTS is\n    present on the API host. Corrected by hand; re-running\n    0-working/probe-domain-security.py will revert it to null.\ndomains:\n- domain: cresta.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy:\
  \ reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cresta/refs/heads/main/security/cresta-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Contact Center
- Contact Center AI
- CCaaS
- Customer Experience
- Conversational AI
- Voice AI
- Agent Assist
- Conversation Intelligence
- Knowledge Agent
- Quality Management
- Real-Time Coaching
- After-Call Automation
- Enterprise AI
- MCP
- Customer Experience AI
- AI Agents
- gRPC
- Speech Analytics
- Enterprise Software
---
