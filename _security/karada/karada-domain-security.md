---
api_specs:
- filename: karada-admin-api-openapi.yml
  format: yaml
  label: Karada AI Admin API
  slug: karada-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karada/refs/heads/main/openapi/karada-admin-api-openapi.yml
- filename: karada-auth-api-openapi.yml
  format: yaml
  label: Karada AI Auth API
  slug: karada-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karada/refs/heads/main/openapi/karada-auth-api-openapi.yml
- filename: karada-billing-api-openapi.yml
  format: yaml
  label: Karada AI Billing API
  slug: karada-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karada/refs/heads/main/openapi/karada-billing-api-openapi.yml
- filename: karada-deployments-api-openapi.yml
  format: yaml
  label: Karada AI Deployments API
  slug: karada-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karada/refs/heads/main/openapi/karada-deployments-api-openapi.yml
- filename: karada-feedback-api-openapi.yml
  format: yaml
  label: Karada AI Feedback API
  slug: karada-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karada/refs/heads/main/openapi/karada-feedback-api-openapi.yml
- filename: karada-gateway-api-openapi.yml
  format: yaml
  label: Karada AI Gateway API
  slug: karada-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karada/refs/heads/main/openapi/karada-gateway-api-openapi.yml
- filename: karada-marketplace-api-openapi.yml
  format: yaml
  label: Karada AI Marketplace API
  slug: karada-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karada/refs/heads/main/openapi/karada-marketplace-api-openapi.yml
- filename: karada-mcp-api-openapi.yml
  format: yaml
  label: Karada AI MCP API
  slug: karada-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karada/refs/heads/main/openapi/karada-mcp-api-openapi.yml
- filename: karada-newsletter-api-openapi.yml
  format: yaml
  label: Karada AI Newsletter API
  slug: karada-newsletter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karada/refs/heads/main/openapi/karada-newsletter-api-openapi.yml
- filename: karada-pricing-api-openapi.yml
  format: yaml
  label: Karada AI Pricing API
  slug: karada-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karada/refs/heads/main/openapi/karada-pricing-api-openapi.yml
- filename: karada-projects-api-openapi.yml
  format: yaml
  label: Karada AI Projects API
  slug: karada-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karada/refs/heads/main/openapi/karada-projects-api-openapi.yml
- filename: karada-registry-api-openapi.yml
  format: yaml
  label: Karada AI Registry API
  slug: karada-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karada/refs/heads/main/openapi/karada-registry-api-openapi.yml
- filename: karada-system-api-openapi.yml
  format: yaml
  label: Karada AI System API
  slug: karada-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karada/refs/heads/main/openapi/karada-system-api-openapi.yml
- filename: karada-teams-api-openapi.yml
  format: yaml
  label: Karada AI Teams API
  slug: karada-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karada/refs/heads/main/openapi/karada-teams-api-openapi.yml
- filename: karada-user-api-openapi.yml
  format: yaml
  label: Karada AI User API
  slug: karada-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karada/refs/heads/main/openapi/karada-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: karada.ai
  spf: true
hosts:
- cert_expires: Nov 28 02:29:46 2026 GMT
  host: karada.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Karada Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Karada AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Karada AI
provider_slug: karada
slug: karada-domain-security
source_filename: karada-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: karada.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 02:29:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: karada.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/karada/refs/heads/main/security/karada-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- AI
- Platform
- MCP
- Automation
---
