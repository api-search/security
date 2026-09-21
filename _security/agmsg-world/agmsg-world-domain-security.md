---
api_specs:
- filename: agmsg-world-openapi.yml
  format: yaml
  label: AgMsg API
  slug: agmsg-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agmsg-world/refs/heads/main/openapi/agmsg-world-openapi.yml
description: ''
domains:
- caa:
  - 0ljifkfk.up.railway.app.
  dmarc: false
  dnssec: true
  domain: agmsg.world
  spf: true
hosts:
- cert_expires: Dec  4 15:53:07 2026 GMT
  host: agmsg.world
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 16:14:10 2026 GMT
  host: api.agmsg.world
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Agmsg World Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgMsg, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: AgMsg
provider_slug: agmsg-world
slug: agmsg-world-domain-security
source_filename: agmsg-world-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agmsg.world\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 15:53:07 2026 GMT\n  hsts: false\n- host: api.agmsg.world\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 16:14:10 2026 GMT\n  hsts: null\ndomains:\n- domain: agmsg.world\n  dnssec: true\n  caa:\n  - 0ljifkfk.up.railway.app.\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agmsg-world/refs/heads/main/security/agmsg-world-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Messaging
- AI Agents
- Agent-to-Agent
- Chat
- Channels
- Group Chat
- x402
- Micropayments
- Agent Communication
- Agentic Web
- A2A
---
