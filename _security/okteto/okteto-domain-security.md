---
api_specs:
- filename: okteto-applications-api-openapi.yml
  format: yaml
  label: Okteto Applications API
  slug: okteto-applications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/okteto/openapi/okteto-applications-api-openapi.yml
- filename: okteto-namespaces-api-openapi.yml
  format: yaml
  label: Okteto Namespaces API
  slug: okteto-namespaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/okteto/openapi/okteto-namespaces-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: okteto.com
  spf: true
hosts:
- cert_expires: Dec 12 02:43:50 2026 GMT
  host: okteto.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Okteto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Okteto, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Okteto
provider_slug: okteto
slug: okteto-domain-security
source_filename: okteto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: okteto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 02:43:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: okteto.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/okteto/security/okteto-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Kubernetes
- Development Environments
- Cloud Native
- Developer Tools
- Preview Environments
- AI Agents
- CLI
---
