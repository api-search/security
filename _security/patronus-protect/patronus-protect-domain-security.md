---
api_specs:
- filename: patronus-protect-openapi.json
  format: json
  label: Patronus Scan API
  slug: patronus-scan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/patronus-protect/refs/heads/main/openapi/patronus-protect-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: patronus.studio
  spf: true
hosts:
- cert_expires: Dec 14 16:39:32 2026 GMT
  host: api.patronus.studio
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 14:53:21 2026 GMT
  host: docs.patronus.studio
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 27 13:09:50 2026 GMT
  host: control.patronus.studio
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Patronus Protect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Patronus Protect, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Patronus Protect
provider_slug: patronus-protect
slug: patronus-protect-domain-security
source_filename: patronus-protect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.patronus.studio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 16:39:32 2026 GMT\n  hsts: false\n- host: docs.patronus.studio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 14:53:21 2026 GMT\n  hsts: false\n- host: control.patronus.studio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 13:09:50 2026 GMT\n  hsts: false\ndomains:\n- domain: patronus.studio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/patronus-protect/refs/heads/main/security/patronus-protect-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI Safety
- Prompt Injection
- Security
- LLM
- Agent-Native
- MCP
- DLP
- PII
- On-Device
- AI Firewall
---
