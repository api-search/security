---
api_specs:
- filename: impact-brand-account-v14-openapi.yml
  format: yaml
  label: Impact Brand API
  slug: brand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/impact/refs/heads/main/openapi/impact-brand-account-v14-openapi.yml
- filename: impact-partner-account-v16-openapi.yml
  format: yaml
  label: Impact Partner API
  slug: partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/impact/refs/heads/main/openapi/impact-partner-account-v16-openapi.yml
- filename: impact-agency-advertisers-v3-openapi.yml
  format: yaml
  label: Impact Agency API
  slug: agency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/impact/refs/heads/main/openapi/impact-agency-advertisers-v3-openapi.yml
- filename: impact-brand-advocate-account-v13-openapi.yml
  format: yaml
  label: Impact Advocate API
  slug: advocate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/impact/refs/heads/main/openapi/impact-brand-advocate-account-v13-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: impact.com
  spf: true
hosts:
- cert_expires: Oct  1 22:13:12 2026 GMT
  host: impact.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 15:33:03 2026 GMT
  host: integrations.impact.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 13:32:39 2026 GMT
  host: mcp.impact.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Impact Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Impact, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Impact
provider_slug: impact
slug: impact-domain-security
source_filename: impact-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: impact.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 22:13:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: integrations.impact.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 15:33:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: mcp.impact.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 13:32:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: impact.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/impact/refs/heads/main/security/impact-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Affiliate
- Partnerships
- Performance Marketing
- Commission
- Tracking
- Creator Economy
- Partner Management
- Referral
- Attribution
- Payouts
- Marketing
- Advertising
- MCP
- Agents
---
