---
api_specs:
- filename: rainbird-technologies-openapi-original.json
  format: json
  label: Rainbird API
  slug: rainbird-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rainbird-technologies/refs/heads/main/openapi/rainbird-technologies-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rainbird.ai
  spf: true
hosts:
- cert_expires: Sep 13 14:26:50 2026 GMT
  host: rainbird.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 23:04:44 2026 GMT
  host: api.rainbird.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 23:23:28 2026 GMT
  host: enterprise-api.rainbird.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rainbird Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rainbird Technologies, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Rainbird Technologies
provider_slug: rainbird-technologies
slug: rainbird-technologies-domain-security
source_filename: rainbird-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rainbird.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 14:26:50 2026 GMT\n  hsts: false\n- host: api.rainbird.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:04:44 2026 GMT\n  hsts: null\n- host: enterprise-api.rainbird.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:23:28 2026 GMT\n  hsts: null\ndomains:\n- domain: rainbird.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rainbird-technologies/refs/heads/main/security/rainbird-technologies-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Decision Automation
- Knowledge Graph
- Symbolic Reasoning
- Explainable AI
- Governance
- RegTech
---
