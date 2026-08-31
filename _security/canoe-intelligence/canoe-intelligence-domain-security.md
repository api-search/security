---
api_specs:
- filename: canoe-intelligence-allocations-api-openapi.yml
  format: yaml
  label: Canoe Intelligence Allocations API
  slug: canoe-intelligence-allocations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-allocations-api-openapi.yml
- filename: canoe-intelligence-authentication-api-openapi.yml
  format: yaml
  label: Canoe Intelligence Authentication API
  slug: canoe-intelligence-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-authentication-api-openapi.yml
- filename: canoe-intelligence-custom-fields-api-openapi.yml
  format: yaml
  label: Canoe Intelligence Custom Fields API
  slug: canoe-intelligence-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-custom-fields-api-openapi.yml
- filename: canoe-intelligence-documents-api-openapi.yml
  format: yaml
  label: Canoe Intelligence Documents API
  slug: canoe-intelligence-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-documents-api-openapi.yml
- filename: canoe-intelligence-funds-api-openapi.yml
  format: yaml
  label: Canoe Intelligence Funds API
  slug: canoe-intelligence-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-funds-api-openapi.yml
- filename: canoe-intelligence-organizations-api-openapi.yml
  format: yaml
  label: Canoe Intelligence Organizations API
  slug: canoe-intelligence-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-organizations-api-openapi.yml
- filename: canoe-intelligence-password-grant-tokens-api-openapi.yml
  format: yaml
  label: Canoe Intelligence Password Grant Tokens API
  slug: canoe-intelligence-password-grant-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-password-grant-tokens-api-openapi.yml
- filename: canoe-intelligence-terms-api-openapi.yml
  format: yaml
  label: Canoe Intelligence Terms API
  slug: canoe-intelligence-terms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-terms-api-openapi.yml
- filename: canoe-intelligence-user-api-openapi.yml
  format: yaml
  label: Canoe Intelligence User API
  slug: canoe-intelligence-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-user-api-openapi.yml
- filename: canoe-intelligence-introduction-api-openapi.yml
  format: yaml
  label: Canoe Intelligence Introduction API
  slug: canoe-intelligence-introduction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-introduction-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: canoeintelligence.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: canoesoftware.com
  spf: true
hosts:
- cert_expires: Sep 15 19:45:07 2026 GMT
  host: canoeintelligence.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 26 23:59:59 2026 GMT
  host: api.canoesoftware.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Canoe Intelligence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Canoe Intelligence, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Canoe Intelligence
provider_slug: canoe-intelligence
slug: canoe-intelligence-domain-security
source_filename: canoe-intelligence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: canoeintelligence.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 19:45:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.canoesoftware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: canoeintelligence.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: canoesoftware.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/security/canoe-intelligence-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- alternative-investments
- private-markets
- document-automation
- data-extraction
- fund-administration
- capital-calls
- k-1-tax-documents
- portfolio-reporting
- Financial-Services
- Fintech
- wealth-management
- institutional-investors
---
