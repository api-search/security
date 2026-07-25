---
api_specs:
- filename: logicgate-access-audit-api-openapi.yml
  format: yaml
  label: LogicGate Access Audit API
  slug: logicgate-access-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logicgate/refs/heads/main/openapi/logicgate-access-audit-api-openapi.yml
- filename: logicgate-application-api-openapi.yml
  format: yaml
  label: LogicGate Application API
  slug: logicgate-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logicgate/refs/heads/main/openapi/logicgate-application-api-openapi.yml
- filename: logicgate-authentication-api-openapi.yml
  format: yaml
  label: LogicGate Authentication API
  slug: logicgate-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logicgate/refs/heads/main/openapi/logicgate-authentication-api-openapi.yml
- filename: logicgate-edge-path-api-openapi.yml
  format: yaml
  label: LogicGate Edge Path API
  slug: logicgate-edge-path-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logicgate/refs/heads/main/openapi/logicgate-edge-path-api-openapi.yml
- filename: logicgate-field-api-openapi.yml
  format: yaml
  label: LogicGate Field API
  slug: logicgate-field-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logicgate/refs/heads/main/openapi/logicgate-field-api-openapi.yml
- filename: logicgate-next-path-api-openapi.yml
  format: yaml
  label: LogicGate Next Path API
  slug: logicgate-next-path-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logicgate/refs/heads/main/openapi/logicgate-next-path-api-openapi.yml
- filename: logicgate-record-api-openapi.yml
  format: yaml
  label: LogicGate Record API
  slug: logicgate-record-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logicgate/refs/heads/main/openapi/logicgate-record-api-openapi.yml
- filename: logicgate-redirect-path-api-openapi.yml
  format: yaml
  label: LogicGate Redirect Path API
  slug: logicgate-redirect-path-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logicgate/refs/heads/main/openapi/logicgate-redirect-path-api-openapi.yml
- filename: logicgate-step-api-openapi.yml
  format: yaml
  label: LogicGate Step API
  slug: logicgate-step-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logicgate/refs/heads/main/openapi/logicgate-step-api-openapi.yml
- filename: logicgate-workflow-api-openapi.yml
  format: yaml
  label: LogicGate Workflow API
  slug: logicgate-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logicgate/refs/heads/main/openapi/logicgate-workflow-api-openapi.yml
- filename: logicgate-workflow-map-api-openapi.yml
  format: yaml
  label: LogicGate Workflow Map API
  slug: logicgate-workflow-map-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logicgate/refs/heads/main/openapi/logicgate-workflow-map-api-openapi.yml
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
