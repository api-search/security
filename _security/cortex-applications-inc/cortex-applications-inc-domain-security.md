---
api_specs:
- filename: cortex-applications-inc-app-api-openapi.yml
  format: yaml
  label: Cortex Applications, Inc. App API
  slug: cortex-applications-inc-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cortex-applications-inc/refs/heads/main/openapi/cortex-applications-inc-app-api-openapi.yml
- filename: cortex-applications-inc-cities-api-openapi.yml
  format: yaml
  label: Cortex Applications, Inc. Cities API
  slug: cortex-applications-inc-cities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cortex-applications-inc/refs/heads/main/openapi/cortex-applications-inc-cities-api-openapi.yml
- filename: cortex-applications-inc-meta-api-openapi.yml
  format: yaml
  label: Cortex Applications, Inc. Meta API
  slug: cortex-applications-inc-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cortex-applications-inc/refs/heads/main/openapi/cortex-applications-inc-meta-api-openapi.yml
- filename: cortex-applications-inc-orgs-api-openapi.yml
  format: yaml
  label: Cortex Applications, Inc. Orgs API
  slug: cortex-applications-inc-orgs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cortex-applications-inc/refs/heads/main/openapi/cortex-applications-inc-orgs-api-openapi.yml
- filename: cortex-applications-inc-repos-api-openapi.yml
  format: yaml
  label: Cortex Applications, Inc. Repos API
  slug: cortex-applications-inc-repos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cortex-applications-inc/refs/heads/main/openapi/cortex-applications-inc-repos-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cortex.io
  spf: true
hosts:
- cert_expires: Nov 16 12:18:13 2026 GMT
  host: www.cortex.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cortex Applications Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cortex Applications, Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Cortex Applications, Inc.
provider_slug: cortex-applications-inc
slug: cortex-applications-inc-domain-security
source_filename: cortex-applications-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cortex.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 12:18:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cortex.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cortex-applications-inc/refs/heads/main/security/cortex-applications-inc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Engineering
- Platform
- Artificial Intelligence
- Developer Productivity
---
