---
api_specs:
- filename: stainless-api-build-target-outputs-api-openapi.yml
  format: yaml
  label: Stainless Build Target Outputs API
  slug: stainless-api-build-target-outputs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stainless-api/refs/heads/main/openapi/stainless-api-build-target-outputs-api-openapi.yml
- filename: stainless-api-builds-api-openapi.yml
  format: yaml
  label: Stainless Builds API
  slug: stainless-api-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stainless-api/refs/heads/main/openapi/stainless-api-builds-api-openapi.yml
- filename: stainless-api-orgs-api-openapi.yml
  format: yaml
  label: Stainless Orgs API
  slug: stainless-api-orgs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stainless-api/refs/heads/main/openapi/stainless-api-orgs-api-openapi.yml
- filename: stainless-api-projects-api-openapi.yml
  format: yaml
  label: Stainless Projects API
  slug: stainless-api-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stainless-api/refs/heads/main/openapi/stainless-api-projects-api-openapi.yml
- filename: stainless-api-user-api-openapi.yml
  format: yaml
  label: Stainless User API
  slug: stainless-api-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stainless-api/refs/heads/main/openapi/stainless-api-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: stainless.com
  spf: true
hosts:
- cert_expires: Aug 16 06:19:18 2026 GMT
  host: www.stainless.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 20:45:39 2026 GMT
  host: api.stainless.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stainless Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stainless, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Stainless
provider_slug: stainless-api
slug: stainless-api-domain-security
source_filename: stainless-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stainless.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 06:19:18 2026 GMT\n  hsts: false\n- host: api.stainless.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 20:45:39 2026 GMT\n  hsts: null\ndomains:\n- domain: stainless.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stainless-api/refs/heads/main/security/stainless-api-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- SDK Generation
- OpenAPI
- API Tooling
- Developer Experience
- MCP
- Model Context Protocol
- Documentation
- Code Generation
- Terraform Provider
- API Reference
- DevTools
- API First
---
