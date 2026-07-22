---
api_specs:
- filename: logicgate-risk-cloud-openapi-original.json
  format: json
  label: Risk Cloud API v2
  slug: risk-cloud-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logicgate/refs/heads/main/openapi/logicgate-risk-cloud-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: logicgate.com
  spf: true
hosts:
- cert_expires: Aug 28 04:13:46 2026 GMT
  host: logicgate.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Logicgate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LogicGate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LogicGate
provider_slug: logicgate
slug: logicgate-domain-security
source_filename: logicgate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: logicgate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 04:13:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: logicgate.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/logicgate/refs/heads/main/security/logicgate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- GRC
- Governance Risk and Compliance
- Risk Management
- Compliance
- Workflow Automation
- Audit
- No-Code
---
