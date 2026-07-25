---
api_specs:
- filename: postman.yaml
  format: yaml
  label: Shareworks Public API
  slug: shareworks-public-api
  spec_type: Postman
  url: https://www.postman.com/
- filename: shareworks-authentication-token-api-openapi.yml
  format: yaml
  label: Shareworks Authentication Token API
  slug: shareworks-authentication-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shareworks/refs/heads/main/openapi/shareworks-authentication-token-api-openapi.yml
- filename: shareworks-authorized-capital-api-openapi.yml
  format: yaml
  label: Shareworks Authorized Capital API
  slug: shareworks-authorized-capital-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shareworks/refs/heads/main/openapi/shareworks-authorized-capital-api-openapi.yml
- filename: shareworks-award-type-api-openapi.yml
  format: yaml
  label: Shareworks Award Type API
  slug: shareworks-award-type-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shareworks/refs/heads/main/openapi/shareworks-award-type-api-openapi.yml
- filename: shareworks-company-api-openapi.yml
  format: yaml
  label: Shareworks Company API
  slug: shareworks-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shareworks/refs/heads/main/openapi/shareworks-company-api-openapi.yml
- filename: shareworks-company-board-api-openapi.yml
  format: yaml
  label: Shareworks Company Board API
  slug: shareworks-company-board-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shareworks/refs/heads/main/openapi/shareworks-company-board-api-openapi.yml
- filename: shareworks-company-integration-api-openapi.yml
  format: yaml
  label: Shareworks Company Integration API
  slug: shareworks-company-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shareworks/refs/heads/main/openapi/shareworks-company-integration-api-openapi.yml
- filename: shareworks-entity-stakeholder-api-openapi.yml
  format: yaml
  label: Shareworks Entity Stakeholder API
  slug: shareworks-entity-stakeholder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shareworks/refs/heads/main/openapi/shareworks-entity-stakeholder-api-openapi.yml
- filename: shareworks-grant-api-openapi.yml
  format: yaml
  label: Shareworks Grant API
  slug: shareworks-grant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shareworks/refs/heads/main/openapi/shareworks-grant-api-openapi.yml
- filename: shareworks-holdings-api-openapi.yml
  format: yaml
  label: Shareworks Holdings API
  slug: shareworks-holdings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shareworks/refs/heads/main/openapi/shareworks-holdings-api-openapi.yml
- filename: shareworks-individual-stakeholder-api-openapi.yml
  format: yaml
  label: Shareworks Individual Stakeholder API
  slug: shareworks-individual-stakeholder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shareworks/refs/heads/main/openapi/shareworks-individual-stakeholder-api-openapi.yml
- filename: shareworks-plan-api-openapi.yml
  format: yaml
  label: Shareworks Plan API
  slug: shareworks-plan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shareworks/refs/heads/main/openapi/shareworks-plan-api-openapi.yml
- filename: shareworks-read-access-api-openapi.yml
  format: yaml
  label: Shareworks Read Access API
  slug: shareworks-read-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shareworks/refs/heads/main/openapi/shareworks-read-access-api-openapi.yml
- filename: shareworks-stock-certificate-api-openapi.yml
  format: yaml
  label: Shareworks Stock Certificate API
  slug: shareworks-stock-certificate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shareworks/refs/heads/main/openapi/shareworks-stock-certificate-api-openapi.yml
- filename: shareworks-stock-filing-api-openapi.yml
  format: yaml
  label: Shareworks Stock Filing API
  slug: shareworks-stock-filing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shareworks/refs/heads/main/openapi/shareworks-stock-filing-api-openapi.yml
- filename: shareworks-vesting-schedule-api-openapi.yml
  format: yaml
  label: Shareworks Vesting Schedule API
  slug: shareworks-vesting-schedule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shareworks/refs/heads/main/openapi/shareworks-vesting-schedule-api-openapi.yml
- filename: shareworks-write-access-api-openapi.yml
  format: yaml
  label: Shareworks Write Access API
  slug: shareworks-write-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shareworks/refs/heads/main/openapi/shareworks-write-access-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: morganstanley.com
  spf: true
- caa:
  - 128 issue "digicert.com"
  - 128 iodef "mailto:hostmaster@shareworks.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: shareworks.com
  spf: true
hosts:
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: www.morganstanley.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb  5 23:59:59 2027 GMT
  host: downloads.shareworks.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: shareworks-api.solium.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shareworks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shareworks, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Shareworks
provider_slug: shareworks
slug: shareworks-domain-security
source_filename: shareworks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.morganstanley.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: downloads.shareworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: null\n- host: shareworks-api.solium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: morganstanley.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: shareworks.com\n  dnssec: false\n  caa:\n  - 128 issue \"digicert.com\"\n  - 128 iodef \"mailto:hostmaster@shareworks.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shareworks/refs/heads/main/security/shareworks-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Equity Compensation
- Stock Options
- RSU
- ESPP
- Employee Equity
- Financial Services
- Morgan Stanley
- Equity Administration
- Private Companies
- Public Companies
---
