---
api_specs:
- filename: node-red-auth-api-openapi.yml
  format: yaml
  label: Node-RED Auth API
  slug: node-red-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/node-red/refs/heads/main/openapi/node-red-auth-api-openapi.yml
- filename: node-red-diagnostics-api-openapi.yml
  format: yaml
  label: Node-RED Diagnostics API
  slug: node-red-diagnostics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/node-red/refs/heads/main/openapi/node-red-diagnostics-api-openapi.yml
- filename: node-red-flow-api-openapi.yml
  format: yaml
  label: Node-RED Flow API
  slug: node-red-flow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/node-red/refs/heads/main/openapi/node-red-flow-api-openapi.yml
- filename: node-red-flows-api-openapi.yml
  format: yaml
  label: Node-RED Flows API
  slug: node-red-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/node-red/refs/heads/main/openapi/node-red-flows-api-openapi.yml
- filename: node-red-nodes-api-openapi.yml
  format: yaml
  label: Node-RED Nodes API
  slug: node-red-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/node-red/refs/heads/main/openapi/node-red-nodes-api-openapi.yml
- filename: node-red-settings-api-openapi.yml
  format: yaml
  label: Node-RED Settings API
  slug: node-red-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/node-red/refs/heads/main/openapi/node-red-settings-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nodered.org
  spf: true
hosts:
- cert_expires: Sep 19 03:05:19 2026 GMT
  host: nodered.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Node Red Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Node-RED, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Node-RED
provider_slug: node-red
slug: node-red-domain-security
source_filename: node-red-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nodered.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 03:05:19 2026 GMT\n  hsts: false\ndomains:\n- domain: nodered.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/node-red/refs/heads/main/security/node-red-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Self-Hosted
- Workflow Automation
- Flow-Based Programming
- IoT
---
