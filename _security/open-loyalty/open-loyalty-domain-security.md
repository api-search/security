---
api_specs:
- filename: open-loyalty-openapi.yml
  format: yaml
  label: Open Loyalty Customer API
  slug: open-loyalty-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-loyalty/refs/heads/main/openapi/open-loyalty-openapi.yml
- filename: open-loyalty-openapi.yml
  format: yaml
  label: Open Loyalty Transactions API
  slug: open-loyalty-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-loyalty/refs/heads/main/openapi/open-loyalty-openapi.yml
- filename: open-loyalty-openapi.yml
  format: yaml
  label: Open Loyalty Points Transfers API
  slug: open-loyalty-points-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-loyalty/refs/heads/main/openapi/open-loyalty-openapi.yml
- filename: open-loyalty-openapi.yml
  format: yaml
  label: Open Loyalty Reward Campaigns API
  slug: open-loyalty-reward-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-loyalty/refs/heads/main/openapi/open-loyalty-openapi.yml
- filename: open-loyalty-openapi.yml
  format: yaml
  label: Open Loyalty Levels API
  slug: open-loyalty-levels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-loyalty/refs/heads/main/openapi/open-loyalty-openapi.yml
- filename: open-loyalty-openapi.yml
  format: yaml
  label: Open Loyalty Earning Rules API
  slug: open-loyalty-earning-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-loyalty/refs/heads/main/openapi/open-loyalty-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openloyalty.io
  spf: true
hosts:
- cert_expires: Aug 15 01:24:47 2026 GMT
  host: www.openloyalty.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 20:41:43 2026 GMT
  host: docs.openloyalty.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: your-instance.openloyalty.io
  https: false
kind: domain-security
layout: security
method: probed
name: Open Loyalty Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Loyalty, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Open Loyalty
provider_slug: open-loyalty
slug: open-loyalty-domain-security
source_filename: open-loyalty-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.openloyalty.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 01:24:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.openloyalty.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 20:41:43 2026 GMT\n  hsts: false\n- host: your-instance.openloyalty.io\n  https: false\ndomains:\n- domain: openloyalty.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-loyalty/refs/heads/main/security/open-loyalty-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Loyalty
- Gamification
- Rewards
- Points
- Loyalty Program
- Customer Engagement
- Headless
- API First
---
