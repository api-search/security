---
api_specs:
- filename: privatedao-org-acquisition-api-openapi.yml
  format: yaml
  label: PrivateDAO Acquisition API
  slug: privatedao-org-acquisition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/privatedao-org/refs/heads/main/openapi/privatedao-org-acquisition-api-openapi.yml
- filename: privatedao-org-agreements-api-openapi.yml
  format: yaml
  label: PrivateDAO Agreements API
  slug: privatedao-org-agreements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/privatedao-org/refs/heads/main/openapi/privatedao-org-agreements-api-openapi.yml
- filename: privatedao-org-discovery-api-openapi.yml
  format: yaml
  label: PrivateDAO Discovery API
  slug: privatedao-org-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/privatedao-org/refs/heads/main/openapi/privatedao-org-discovery-api-openapi.yml
- filename: privatedao-org-health-api-openapi.yml
  format: yaml
  label: PrivateDAO Health API
  slug: privatedao-org-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/privatedao-org/refs/heads/main/openapi/privatedao-org-health-api-openapi.yml
- filename: privatedao-org-jobs-api-openapi.yml
  format: yaml
  label: PrivateDAO Jobs API
  slug: privatedao-org-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/privatedao-org/refs/heads/main/openapi/privatedao-org-jobs-api-openapi.yml
- filename: privatedao-org-logistics-api-openapi.yml
  format: yaml
  label: PrivateDAO Logistics API
  slug: privatedao-org-logistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/privatedao-org/refs/heads/main/openapi/privatedao-org-logistics-api-openapi.yml
- filename: privatedao-org-marketplace-api-openapi.yml
  format: yaml
  label: PrivateDAO Marketplace API
  slug: privatedao-org-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/privatedao-org/refs/heads/main/openapi/privatedao-org-marketplace-api-openapi.yml
- filename: privatedao-org-pricing-api-openapi.yml
  format: yaml
  label: PrivateDAO Pricing API
  slug: privatedao-org-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/privatedao-org/refs/heads/main/openapi/privatedao-org-pricing-api-openapi.yml
- filename: privatedao-org-proof-workflows-api-openapi.yml
  format: yaml
  label: PrivateDAO Proof Workflows API
  slug: privatedao-org-proof-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/privatedao-org/refs/heads/main/openapi/privatedao-org-proof-workflows-api-openapi.yml
- filename: privatedao-org-receipts-api-openapi.yml
  format: yaml
  label: PrivateDAO Receipts API
  slug: privatedao-org-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/privatedao-org/refs/heads/main/openapi/privatedao-org-receipts-api-openapi.yml
- filename: privatedao-org-referrals-api-openapi.yml
  format: yaml
  label: PrivateDAO Referrals API
  slug: privatedao-org-referrals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/privatedao-org/refs/heads/main/openapi/privatedao-org-referrals-api-openapi.yml
- filename: privatedao-org-registry-api-openapi.yml
  format: yaml
  label: PrivateDAO Registry API
  slug: privatedao-org-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/privatedao-org/refs/heads/main/openapi/privatedao-org-registry-api-openapi.yml
- filename: privatedao-org-revenue-api-openapi.yml
  format: yaml
  label: PrivateDAO Revenue API
  slug: privatedao-org-revenue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/privatedao-org/refs/heads/main/openapi/privatedao-org-revenue-api-openapi.yml
- filename: privatedao-org-services-api-openapi.yml
  format: yaml
  label: PrivateDAO Services API
  slug: privatedao-org-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/privatedao-org/refs/heads/main/openapi/privatedao-org-services-api-openapi.yml
- filename: privatedao-org-treasury-api-openapi.yml
  format: yaml
  label: PrivateDAO Treasury API
  slug: privatedao-org-treasury-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/privatedao-org/refs/heads/main/openapi/privatedao-org-treasury-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: privatedao.org
  spf: true
hosts:
- cert_expires: Nov  7 00:09:26 2026 GMT
  host: privatedao.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  1 23:59:59 2027 GMT
  host: agents.privatedao.org
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 15:22:06 2026 GMT
  host: api.privatedao.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Privatedao Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PrivateDAO, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: PrivateDAO
provider_slug: privatedao-org
slug: privatedao-org-domain-security
source_filename: privatedao-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: privatedao.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 00:09:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: agents.privatedao.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  1 23:59:59 2027 GMT\n  hsts: null\n- host: api.privatedao.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 15:22:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: privatedao.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/privatedao-org/refs/heads/main/security/privatedao-org-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Agents
- A2A
- MCP
- Verification
- Zero-Knowledge Proofs
- Solana
- Blockchain
- Payments
- Marketplace
- Privacy
- Governance
- Treasury
---
