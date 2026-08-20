---
api_specs:
- filename: stainless-build-target-outputs-api-openapi.yml
  format: yaml
  label: Stainless Build Target Outputs API
  slug: stainless-build-target-outputs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stainless/refs/heads/main/openapi/stainless-build-target-outputs-api-openapi.yml
- filename: stainless-builds-api-openapi.yml
  format: yaml
  label: Stainless Builds API
  slug: stainless-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stainless/refs/heads/main/openapi/stainless-builds-api-openapi.yml
- filename: stainless-orgs-api-openapi.yml
  format: yaml
  label: Stainless Orgs API
  slug: stainless-orgs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stainless/refs/heads/main/openapi/stainless-orgs-api-openapi.yml
- filename: stainless-projects-api-openapi.yml
  format: yaml
  label: Stainless Projects API
  slug: stainless-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stainless/refs/heads/main/openapi/stainless-projects-api-openapi.yml
- filename: stainless-user-api-openapi.yml
  format: yaml
  label: Stainless User API
  slug: stainless-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stainless/refs/heads/main/openapi/stainless-user-api-openapi.yml
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
name: Stainless Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stainless, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Stainless
provider_slug: stainless
slug: stainless-domain-security
source_filename: stainless-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stainless.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 06:19:18 2026 GMT\n  hsts: false\n- host: api.stainless.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 20:45:39 2026 GMT\n  hsts: null\ndomains:\n- domain: stainless.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stainless/refs/heads/main/security/stainless-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Code Generation
- Documentation
- Developer Experience
- MCP
- Platform
- SDK
- Terraform
---
