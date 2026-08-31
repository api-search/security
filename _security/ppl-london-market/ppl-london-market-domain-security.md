---
api_specs:
- filename: ppl-london-market-contract-api-openapi.yml
  format: yaml
  label: PPL Contract API
  slug: ppl-london-market-contract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppl-london-market/refs/heads/main/openapi/ppl-london-market-contract-api-openapi.yml
- filename: ppl-london-market-document-api-openapi.yml
  format: yaml
  label: PPL Document API
  slug: ppl-london-market-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppl-london-market/refs/heads/main/openapi/ppl-london-market-document-api-openapi.yml
- filename: ppl-london-market-health-api-openapi.yml
  format: yaml
  label: PPL Health API
  slug: ppl-london-market-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppl-london-market/refs/heads/main/openapi/ppl-london-market-health-api-openapi.yml
- filename: ppl-london-market-negotiation-api-openapi.yml
  format: yaml
  label: PPL Negotiation API
  slug: ppl-london-market-negotiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppl-london-market/refs/heads/main/openapi/ppl-london-market-negotiation-api-openapi.yml
- filename: ppl-london-market-notification-api-openapi.yml
  format: yaml
  label: PPL Notification API
  slug: ppl-london-market-notification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppl-london-market/refs/heads/main/openapi/ppl-london-market-notification-api-openapi.yml
- filename: ppl-london-market-organisation-api-openapi.yml
  format: yaml
  label: PPL Organisation API
  slug: ppl-london-market-organisation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppl-london-market/refs/heads/main/openapi/ppl-london-market-organisation-api-openapi.yml
- filename: ppl-london-market-participation-api-openapi.yml
  format: yaml
  label: PPL Participation API
  slug: ppl-london-market-participation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppl-london-market/refs/heads/main/openapi/ppl-london-market-participation-api-openapi.yml
- filename: ppl-london-market-placement-api-openapi.yml
  format: yaml
  label: PPL Placement API
  slug: ppl-london-market-placement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppl-london-market/refs/heads/main/openapi/ppl-london-market-placement-api-openapi.yml
- filename: ppl-london-market-programme-api-openapi.yml
  format: yaml
  label: PPL Programme API
  slug: ppl-london-market-programme-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppl-london-market/refs/heads/main/openapi/ppl-london-market-programme-api-openapi.yml
- filename: ppl-london-market-section-api-openapi.yml
  format: yaml
  label: PPL Section API
  slug: ppl-london-market-section-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppl-london-market/refs/heads/main/openapi/ppl-london-market-section-api-openapi.yml
- filename: ppl-london-market-submission-api-openapi.yml
  format: yaml
  label: PPL Submission API
  slug: ppl-london-market-submission-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppl-london-market/refs/heads/main/openapi/ppl-london-market-submission-api-openapi.yml
- filename: ppl-london-market-transaction-api-openapi.yml
  format: yaml
  label: PPL Transaction API
  slug: ppl-london-market-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppl-london-market/refs/heads/main/openapi/ppl-london-market-transaction-api-openapi.yml
- filename: ppl-london-market-version-api-openapi.yml
  format: yaml
  label: PPL Version API
  slug: ppl-london-market-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppl-london-market/refs/heads/main/openapi/ppl-london-market-version-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: placingplatformlimited.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pplnextgen.com
  spf: true
hosts:
- cert_expires: Sep  3 14:24:46 2026 GMT
  host: placingplatformlimited.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: developer.pplnextgen.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: api.londonmarketgroup.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ppl London Market Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PPL, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PPL
provider_slug: ppl-london-market
slug: ppl-london-market-domain-security
source_filename: ppl-london-market-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: placingplatformlimited.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 14:24:46 2026 GMT\n  hsts: false\n- host: developer.pplnextgen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: api.londonmarketgroup.co.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: placingplatformlimited.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: pplnextgen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ppl-london-market/refs/heads/main/security/ppl-london-market-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- United Kingdom
- London Market
- Lloyd's of London
- Reinsurance
- Commercial Insurance
- Brokers
- Underwriting
- Placement
- Market Infrastructure
- ACORD
- Electronic Placing
---
