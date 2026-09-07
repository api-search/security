---
api_specs:
- filename: ballerina-packages-api-openapi.yml
  format: yaml
  label: Ballerina Packages API
  slug: ballerina-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ballerina/refs/heads/main/openapi/ballerina-packages-api-openapi.yml
- filename: ballerina-connectors-api-openapi.yml
  format: yaml
  label: Ballerina Connectors API
  slug: ballerina-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ballerina/refs/heads/main/openapi/ballerina-connectors-api-openapi.yml
- filename: ballerina-triggers-api-openapi.yml
  format: yaml
  label: Ballerina Triggers API
  slug: ballerina-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ballerina/refs/heads/main/openapi/ballerina-triggers-api-openapi.yml
- filename: ballerina-docs-api-openapi.yml
  format: yaml
  label: Ballerina Docs API
  slug: ballerina-docs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ballerina/refs/heads/main/openapi/ballerina-docs-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: ballerina.io
  spf: true
hosts:
- cert_expires: Nov 22 16:20:50 2026 GMT
  host: ballerina.io
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: api.central.ballerina.io
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Ballerina Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ballerina, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Ballerina
provider_slug: ballerina
slug: ballerina-domain-security
source_filename: ballerina-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ballerina.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 16:20:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: api.central.ballerina.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: ballerina.io\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ballerina/refs/heads/main/security/ballerina-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Integration
- Orchestrations
- Open-Source
- Programming Language
- Package Registry
- Developer Tools
- Code Generation
- Agent Skills
---
