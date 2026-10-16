---
api_specs:
- filename: cosuno-awarded-bids-api-openapi.yml
  format: yaml
  label: Cosuno Awarded Bids API
  slug: cosuno-awarded-bids-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosuno/refs/heads/main/openapi/cosuno-awarded-bids-api-openapi.yml
- filename: cosuno-bid-package-custom-fields-api-openapi.yml
  format: yaml
  label: Cosuno Bid Package Custom Fields API
  slug: cosuno-bid-package-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosuno/refs/heads/main/openapi/cosuno-bid-package-custom-fields-api-openapi.yml
- filename: cosuno-bid-packages-api-openapi.yml
  format: yaml
  label: Cosuno Bid Packages API
  slug: cosuno-bid-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosuno/refs/heads/main/openapi/cosuno-bid-packages-api-openapi.yml
- filename: cosuno-bid-requests-api-openapi.yml
  format: yaml
  label: Cosuno Bid Requests API
  slug: cosuno-bid-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosuno/refs/heads/main/openapi/cosuno-bid-requests-api-openapi.yml
- filename: cosuno-bids-api-openapi.yml
  format: yaml
  label: Cosuno Bids API
  slug: cosuno-bids-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosuno/refs/heads/main/openapi/cosuno-bids-api-openapi.yml
- filename: cosuno-company-api-openapi.yml
  format: yaml
  label: Cosuno Company API
  slug: cosuno-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosuno/refs/heads/main/openapi/cosuno-company-api-openapi.yml
- filename: cosuno-current-user-api-openapi.yml
  format: yaml
  label: Cosuno Current User API
  slug: cosuno-current-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosuno/refs/heads/main/openapi/cosuno-current-user-api-openapi.yml
- filename: cosuno-offices-api-openapi.yml
  format: yaml
  label: Cosuno Offices API
  slug: cosuno-offices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosuno/refs/heads/main/openapi/cosuno-offices-api-openapi.yml
- filename: cosuno-project-costs-api-openapi.yml
  format: yaml
  label: Cosuno Project Costs API
  slug: cosuno-project-costs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosuno/refs/heads/main/openapi/cosuno-project-costs-api-openapi.yml
- filename: cosuno-project-custom-fields-api-openapi.yml
  format: yaml
  label: Cosuno Project Custom Fields API
  slug: cosuno-project-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosuno/refs/heads/main/openapi/cosuno-project-custom-fields-api-openapi.yml
- filename: cosuno-projects-api-openapi.yml
  format: yaml
  label: Cosuno Projects API
  slug: cosuno-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosuno/refs/heads/main/openapi/cosuno-projects-api-openapi.yml
- filename: cosuno-subcontractor-custom-fields-api-openapi.yml
  format: yaml
  label: Cosuno Subcontractor Custom Fields API
  slug: cosuno-subcontractor-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosuno/refs/heads/main/openapi/cosuno-subcontractor-custom-fields-api-openapi.yml
- filename: cosuno-subcontractor-reviews-api-openapi.yml
  format: yaml
  label: Cosuno Subcontractor Reviews API
  slug: cosuno-subcontractor-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosuno/refs/heads/main/openapi/cosuno-subcontractor-reviews-api-openapi.yml
- filename: cosuno-subcontractors-api-openapi.yml
  format: yaml
  label: Cosuno Subcontractors API
  slug: cosuno-subcontractors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosuno/refs/heads/main/openapi/cosuno-subcontractors-api-openapi.yml
- filename: cosuno-users-api-openapi.yml
  format: yaml
  label: Cosuno Users API
  slug: cosuno-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosuno/refs/heads/main/openapi/cosuno-users-api-openapi.yml
- filename: cosuno-webhooks-api-openapi.yml
  format: yaml
  label: Cosuno Webhooks API
  slug: cosuno-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosuno/refs/heads/main/openapi/cosuno-webhooks-api-openapi.yml
- filename: cosuno-work-categories-api-openapi.yml
  format: yaml
  label: Cosuno Work Categories API
  slug: cosuno-work-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosuno/refs/heads/main/openapi/cosuno-work-categories-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cosuno.com
  spf: true
hosts:
- cert_expires: Apr 22 23:59:59 2027 GMT
  host: www.cosuno.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cosuno Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cosuno, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cosuno
provider_slug: cosuno
slug: cosuno-domain-security
source_filename: cosuno-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cosuno.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cosuno.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cosuno/refs/heads/main/security/cosuno-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Construction
- Marketplace
- AI
- Tendering
- Germany
---
