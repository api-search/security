---
api_specs:
- filename: agent4-io-api-openapi.json
  format: json
  label: chatagent-platform Api API
  slug: chatagent-platform-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agent4-io/openapi/_original/agent4-io-api-openapi.json
description: ''
domains:
- caa:
  - dev.agent4.io.
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: agent4.io
  spf: false
hosts:
- cert_expires: Dec 14 15:01:54 2026 GMT
  host: agent4.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agent4 Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agent4.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: Agent4.io
provider_slug: agent4-io
slug: agent4-io-domain-security
source_filename: agent4-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agent4.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 15:01:54 2026 GMT\n  hsts: false\ndomains:\n- domain: agent4.io\n  dnssec: true\n  caa:\n  - dev.agent4.io.\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/agent4-io/security/agent4-io-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Automation
- Customer Engagement
- Software-as-a-Service
- Agent Platform
---
