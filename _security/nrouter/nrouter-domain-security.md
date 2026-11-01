---
api_specs:
- filename: nrouter-openapi-generated.yml
  format: yaml
  label: CloudAct API
  slug: nrouter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nrouter/openapi/_ae-authored/nrouter-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:support@nrouter.ai"
  - 0 issuewild "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nrouter.ai
  spf: true
hosts:
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: nrouter.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nrouter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CloudAct, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CloudAct
provider_slug: nrouter
slug: nrouter-domain-security
source_filename: nrouter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nrouter.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: nrouter.ai\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:support@nrouter.ai\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/nrouter/security/nrouter-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- LLM Gateway
- AI Infrastructure
- Smart Routing
- Token Management
---
