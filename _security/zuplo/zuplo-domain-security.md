---
api_specs:
- filename: zuplo-api-keys-buckets-api-openapi.yml
  format: yaml
  label: Zuplo API Keys - Buckets API
  slug: zuplo-api-keys-buckets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuplo/refs/heads/main/openapi/zuplo-api-keys-buckets-api-openapi.yml
- filename: zuplo-api-keys-consumers-api-openapi.yml
  format: yaml
  label: Zuplo API Keys - Consumers API
  slug: zuplo-api-keys-consumers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuplo/refs/heads/main/openapi/zuplo-api-keys-consumers-api-openapi.yml
- filename: zuplo-api-keys-keys-api-openapi.yml
  format: yaml
  label: Zuplo API Keys - Keys API
  slug: zuplo-api-keys-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuplo/refs/heads/main/openapi/zuplo-api-keys-keys-api-openapi.yml
- filename: zuplo-api-keys-managers-api-openapi.yml
  format: yaml
  label: Zuplo API Keys - Managers API
  slug: zuplo-api-keys-managers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuplo/refs/heads/main/openapi/zuplo-api-keys-managers-api-openapi.yml
- filename: zuplo-audit-logs-api-openapi.yml
  format: yaml
  label: Zuplo Audit Logs API
  slug: zuplo-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuplo/refs/heads/main/openapi/zuplo-audit-logs-api-openapi.yml
- filename: zuplo-custom-domains-api-openapi.yml
  format: yaml
  label: Zuplo Custom Domains API
  slug: zuplo-custom-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuplo/refs/heads/main/openapi/zuplo-custom-domains-api-openapi.yml
- filename: zuplo-deployments-api-openapi.yml
  format: yaml
  label: Zuplo Deployments API
  slug: zuplo-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuplo/refs/heads/main/openapi/zuplo-deployments-api-openapi.yml
- filename: zuplo-mcp-servers-api-openapi.yml
  format: yaml
  label: Zuplo MCP Servers API
  slug: zuplo-mcp-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuplo/refs/heads/main/openapi/zuplo-mcp-servers-api-openapi.yml
- filename: zuplo-openapi-api-openapi.yml
  format: yaml
  label: Zuplo Openapi API
  slug: zuplo-openapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuplo/refs/heads/main/openapi/zuplo-openapi-api-openapi.yml
- filename: zuplo-tunnel-services-api-openapi.yml
  format: yaml
  label: Zuplo Tunnel Services API
  slug: zuplo-tunnel-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuplo/refs/heads/main/openapi/zuplo-tunnel-services-api-openapi.yml
- filename: zuplo-tunnels-api-openapi.yml
  format: yaml
  label: Zuplo Tunnels API
  slug: zuplo-tunnels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuplo/refs/heads/main/openapi/zuplo-tunnels-api-openapi.yml
- filename: zuplo-variables-api-openapi.yml
  format: yaml
  label: Zuplo Variables API
  slug: zuplo-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuplo/refs/heads/main/openapi/zuplo-variables-api-openapi.yml
- filename: zuplo-who-am-i-api-openapi.yml
  format: yaml
  label: Zuplo Who Am I API
  slug: zuplo-who-am-i-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuplo/refs/heads/main/openapi/zuplo-who-am-i-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: zuplo.com
  spf: true
hosts:
- cert_expires: Aug 17 03:16:39 2026 GMT
  host: zuplo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 13:23:10 2026 GMT
  host: dev.zuplo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zuplo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zuplo, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Zuplo
provider_slug: zuplo
slug: zuplo-domain-security
source_filename: zuplo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zuplo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 03:16:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: dev.zuplo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 13:23:10 2026 GMT\n  hsts: null\ndomains:\n- domain: zuplo.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zuplo/refs/heads/main/security/zuplo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI Gateway
- API Management
- Gateways
- Platform
---
