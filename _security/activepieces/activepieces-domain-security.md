---
api_specs:
- filename: activepieces.json
  format: json
  label: Activepieces API
  slug: activepieces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/openapi/activepieces.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: activepieces.com
  spf: true
hosts:
- cert_expires: Aug 31 09:42:47 2026 GMT
  host: www.activepieces.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 15:15:31 2026 GMT
  host: cloud.activepieces.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Activepieces Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Activepieces, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Activepieces
provider_slug: activepieces
slug: activepieces-domain-security
source_filename: activepieces-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.activepieces.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 09:42:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cloud.activepieces.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 15:15:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: activepieces.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/security/activepieces-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Automation
- No-Code
- Open Source
- Workflow
- AI Agents
- MCP
---
