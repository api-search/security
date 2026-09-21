---
api_specs:
- filename: clix-so-openapi.yml
  format: yaml
  label: Clix External API
  slug: clix-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clix-so/refs/heads/main/openapi/clix-so-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: clix.so
  spf: true
hosts:
- cert_expires: Dec 18 17:18:31 2026 GMT
  host: clix.so
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 10:38:42 2026 GMT
  host: api.clix.so
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Clix So Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clix, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Clix
provider_slug: clix-so
slug: clix-so-domain-security
source_filename: clix-so-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clix.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 17:18:31 2026 GMT\n  hsts: false\n- host: api.clix.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 10:38:42 2026 GMT\n  hsts: null\ndomains:\n- domain: clix.so\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clix-so/refs/heads/main/security/clix-so-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Push Notifications
- Mobile
- Messaging
- Campaigns
- Event Tracking
- Customer Engagement
- A2A
- MCP
- Agents
- SDK
- United States
- Company
---
