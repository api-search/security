---
api_specs:
- filename: kubermatic-apis-api-openapi.yml
  format: yaml
  label: Kubermatic APIs API
  slug: kubermatic-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubermatic/refs/heads/main/openapi/kubermatic-apis-api-openapi.yml
- filename: kubermatic-auth-api-openapi.yml
  format: yaml
  label: Kubermatic Auth API
  slug: kubermatic-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubermatic/refs/heads/main/openapi/kubermatic-auth-api-openapi.yml
- filename: kubermatic-clusters-api-openapi.yml
  format: yaml
  label: Kubermatic Clusters API
  slug: kubermatic-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubermatic/refs/heads/main/openapi/kubermatic-clusters-api-openapi.yml
- filename: kubermatic-healthz-api-openapi.yml
  format: yaml
  label: Kubermatic Healthz API
  slug: kubermatic-healthz-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubermatic/refs/heads/main/openapi/kubermatic-healthz-api-openapi.yml
- filename: kubermatic-kubermatic-api-api-openapi.yml
  format: yaml
  label: Kubermatic Kubermatic API
  slug: kubermatic-kubermatic-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubermatic/refs/heads/main/openapi/kubermatic-kubermatic-api-api-openapi.yml
- filename: kubermatic-kubermatic-api-openapi.yml
  format: yaml
  label: Kubermatic Kubermatic API
  slug: kubermatic-kubermatic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubermatic/refs/heads/main/openapi/kubermatic-kubermatic-api-openapi.yml
- filename: kubermatic-mcp-api-openapi.yml
  format: yaml
  label: Kubermatic MCP API
  slug: kubermatic-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubermatic/refs/heads/main/openapi/kubermatic-mcp-api-openapi.yml
- filename: kubermatic-metrics-api-openapi.yml
  format: yaml
  label: Kubermatic Metrics API
  slug: kubermatic-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubermatic/refs/heads/main/openapi/kubermatic-metrics-api-openapi.yml
- filename: kubermatic-well-known-api-openapi.yml
  format: yaml
  label: Kubermatic .well Known API
  slug: kubermatic-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubermatic/refs/heads/main/openapi/kubermatic-well-known-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: kubermatic.com
  spf: true
hosts:
- cert_expires: Nov 20 02:16:38 2026 GMT
  host: www.kubermatic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kubermatic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kubermatic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Kubermatic
provider_slug: kubermatic
slug: kubermatic-domain-security
source_filename: kubermatic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kubermatic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 02:16:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kubermatic.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kubermatic/refs/heads/main/security/kubermatic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Kubernetes
- Multi-Cloud
- Platform
- Artificial Intelligence
---
