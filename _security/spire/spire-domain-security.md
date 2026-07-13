---
api_specs:
- filename: spire-workload-asyncapi.yml
  format: yaml
  label: SPIRE Workload API
  slug: spire-workload-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/spire/refs/heads/main/asyncapi/spire-workload-asyncapi.yml
- filename: spire-health-openapi.yml
  format: yaml
  label: SPIRE Agent API
  slug: spire-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spire/refs/heads/main/openapi/spire-health-openapi.yml
- filename: spire-oidc-discovery-openapi.yml
  format: yaml
  label: SPIRE OIDC Discovery API
  slug: spire-oidc-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spire/refs/heads/main/openapi/spire-oidc-discovery-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: spiffe.io
  spf: false
hosts:
- cert_expires: Aug 15 05:17:40 2026 GMT
  host: spiffe.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spire Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SPIRE, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: SPIRE
provider_slug: spire
slug: spire-domain-security
source_filename: spire-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spiffe.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 05:17:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: spiffe.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spire/refs/heads/main/security/spire-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Authentication
- Cloud Native
- Graduated
- Identity
- Security
- Zero Trust
---
