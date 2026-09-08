---
api_specs:
- filename: facets-control-plane-openapi.yml
  format: yaml
  label: Facets Control Plane API
  slug: facets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facets/refs/heads/main/openapi/facets-control-plane-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: facets.cloud
  spf: true
hosts:
- cert_expires: Nov 21 16:23:15 2026 GMT
  host: www.facets.cloud
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  3 01:13:14 2026 GMT
  host: facetsdemo.console.facets.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Facets Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Facets, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Facets
provider_slug: facets
slug: facets-domain-security
source_filename: facets-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.facets.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 16:23:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: facetsdemo.console.facets.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 01:13:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: facets.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/facets/refs/heads/main/security/facets-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automation
- Infrastructure
- Orchestration
- Platform Engineering
- DevOps
- Internal Developer Platform
- Terraform
- Kubernetes
- Continuous Delivery
- AI Agents
---
