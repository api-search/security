---
api_specs:
- filename: signadot-openapi-original.yml
  format: yaml
  label: Signadot API
  slug: signadot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signadot/refs/heads/main/openapi/signadot-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: signadot.com
  spf: true
hosts:
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: signadot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 20 23:59:59 2027 GMT
  host: api.signadot.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Signadot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Signadot, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Signadot
provider_slug: signadot
slug: signadot-domain-security
source_filename: signadot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: signadot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.signadot.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 20 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: signadot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/signadot/refs/heads/main/security/signadot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Developer Tools
- Kubernetes
- Testing
- Ephemeral Environments
- Microservices
- Preview Environments
- Agentic Development
- Continuous Integration
- Developer Experience
---
