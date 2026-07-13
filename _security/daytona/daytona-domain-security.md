---
api_specs:
- filename: openapi.json
  format: json
  label: Daytona Sandbox API
  slug: sandbox-api
  spec_type: OpenAPI
  url: https://app.daytona.io/api/docs/openapi.json
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:security@daytona.io"
  - 0 issue "amazontrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: daytona.io
  spf: true
hosts:
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: www.daytona.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 13 23:59:59 2027 GMT
  host: app.daytona.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Daytona Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Daytona, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Daytona
provider_slug: daytona
slug: daytona-domain-security
source_filename: daytona-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.daytona.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.daytona.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: daytona.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@daytona.io\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/daytona/refs/heads/main/security/daytona-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sandboxes
- Secure Execution
- AI Agents
- Coding Agents
- Code Interpreter
- Snapshots
- Multi-Region
- HIPAA
- SOC 2
- GDPR
- Python
- TypeScript
- Open Source
- LSP
---
