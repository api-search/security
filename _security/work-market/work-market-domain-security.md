---
api_specs:
- filename: work-market-addressbook-api-openapi.yml
  format: yaml
  label: Work Market Addressbook API
  slug: work-market-addressbook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/work-market/refs/heads/main/openapi/work-market-addressbook-api-openapi.yml
- filename: work-market-assignments-api-openapi.yml
  format: yaml
  label: Work Market Assignments API
  slug: work-market-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/work-market/refs/heads/main/openapi/work-market-assignments-api-openapi.yml
- filename: work-market-authorization-api-openapi.yml
  format: yaml
  label: Work Market Authorization API
  slug: work-market-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/work-market/refs/heads/main/openapi/work-market-authorization-api-openapi.yml
- filename: work-market-constants-api-openapi.yml
  format: yaml
  label: Work Market Constants API
  slug: work-market-constants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/work-market/refs/heads/main/openapi/work-market-constants-api-openapi.yml
- filename: work-market-custom-fields-api-openapi.yml
  format: yaml
  label: Work Market Custom Fields API
  slug: work-market-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/work-market/refs/heads/main/openapi/work-market-custom-fields-api-openapi.yml
- filename: work-market-labels-api-openapi.yml
  format: yaml
  label: Work Market Labels API
  slug: work-market-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/work-market/refs/heads/main/openapi/work-market-labels-api-openapi.yml
- filename: work-market-locations-api-openapi.yml
  format: yaml
  label: Work Market Locations API
  slug: work-market-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/work-market/refs/heads/main/openapi/work-market-locations-api-openapi.yml
- filename: work-market-projects-api-openapi.yml
  format: yaml
  label: Work Market Projects API
  slug: work-market-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/work-market/refs/heads/main/openapi/work-market-projects-api-openapi.yml
- filename: work-market-talent-pools-api-openapi.yml
  format: yaml
  label: Work Market Talent Pools API
  slug: work-market-talent-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/work-market/refs/heads/main/openapi/work-market-talent-pools-api-openapi.yml
- filename: work-market-updatecheckin-api-openapi.yml
  format: yaml
  label: Work Market UpdateCheckIn API
  slug: work-market-updatecheckin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/work-market/refs/heads/main/openapi/work-market-updatecheckin-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "digicert.com"
  - 0 issue "comodoca.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: workmarket.com
  spf: true
hosts:
- cert_expires: Dec 21 23:59:59 2026 GMT
  host: workmarket.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 22:08:27 2026 GMT
  host: employer-api.workmarket.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 21 23:59:59 2026 GMT
  host: www.workmarket.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Work Market Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Work Market, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Work Market
provider_slug: work-market
slug: work-market-domain-security
source_filename: work-market-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: workmarket.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: employer-api.workmarket.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 22:08:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.workmarket.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: workmarket.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/work-market/refs/heads/main/security/work-market-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Workforce Management
- Contractors
- Freelance
- Gig Economy
- Human Resources
- Payments
- Field Services
- Staffing
---
