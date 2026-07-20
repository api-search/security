---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: glue.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gluegroups.com
  spf: true
hosts:
- cert_expires: Aug 19 23:21:00 2026 GMT
  host: glue.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 03:51:27 2026 GMT
  host: docs.glue.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  6 23:59:59 2027 GMT
  host: api.gluegroups.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Glue Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Glue, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Glue
provider_slug: glue
slug: glue-domain-security
source_filename: glue-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: glue.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 23:21:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.glue.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 03:51:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.gluegroups.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  6 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: glue.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: gluegroups.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glue/refs/heads/main/security/glue-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- SaaS
- Team Communication
- Messaging
- Collaboration
- GraphQL
- Webhooks
- MCP
- Productivity
- AI Agents
---
