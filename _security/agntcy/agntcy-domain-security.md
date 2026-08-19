---
api_specs:
- filename: agntcy-oasf-schema-swagger.json
  format: json
  label: OASF Schema API
  slug: oasf-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agntcy/refs/heads/main/openapi/agntcy-oasf-schema-swagger.json
- filename: agntcy-acp-openapi.json
  format: json
  label: Agent Connect Protocol (ACP)
  slug: agent-connect-protocol-acp
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agntcy/refs/heads/main/openapi/agntcy-acp-openapi.json
- filename: agntcy-identity-service-openapi.yaml
  format: yaml
  label: AGNTCY Identity Service API
  slug: agntcy-identity-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agntcy/refs/heads/main/openapi/agntcy-identity-service-openapi.yaml
- filename: agntcy-identity-node-openapi.yaml
  format: yaml
  label: AGNTCY Identity Node API
  slug: agntcy-identity-node-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agntcy/refs/heads/main/openapi/agntcy-identity-node-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: agntcy.org
  spf: true
- caa:
  - 0 issue "pki.goog"
  - 128 issuewild "ssl.com"
  - 0 issue "digicert.com"
  - 128 issuewild "digicert.com"
  - 0 issue "letsencrypt.org"
  - 128 issuewild "identrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cisco.com
  spf: true
hosts:
- cert_expires: Nov  7 05:29:51 2026 GMT
  host: agntcy.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 13 18:26:40 2027 GMT
  host: outshift.cisco.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: 0.0.0.0
  https: false
kind: domain-security
layout: security
method: probed
name: Agntcy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AGNTCY, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AGNTCY
provider_slug: agntcy
slug: agntcy-domain-security
source_filename: agntcy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agntcy.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 05:29:51 2026 GMT\n  hsts: false\n- host: outshift.cisco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 18:26:40 2027 GMT\n  hsts: false\n- host: 0.0.0.0\n  https: false\ndomains:\n- domain: agntcy.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: cisco.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 128 issuewild \"ssl.com\"\n  - 0 issue \"digicert.com\"\n  - 128 issuewild \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 128 issuewild \"identrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agntcy/refs/heads/main/security/agntcy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI Agents
- Interoperability
- Specification
- Open Source
- Agent Discovery
- Identity
- Agent Directory
- Model Context Protocol
- A2A
- OpenAPI
- gRPC
- Protocol Buffers
- Verifiable Credentials
- Schema
- Taxonomy
- Messaging
- Observability
- Linux Foundation
---
