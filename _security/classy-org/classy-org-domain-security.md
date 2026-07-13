---
api_specs:
- filename: classy-org-openapi.yml
  format: yaml
  label: Classy Organizations API
  slug: classy-org-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/classy-org/refs/heads/main/openapi/classy-org-openapi.yml
- filename: classy-org-openapi.yml
  format: yaml
  label: Classy Campaigns API
  slug: classy-org-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/classy-org/refs/heads/main/openapi/classy-org-openapi.yml
- filename: classy-org-openapi.yml
  format: yaml
  label: Classy Fundraising Pages API
  slug: classy-org-fundraising-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/classy-org/refs/heads/main/openapi/classy-org-openapi.yml
- filename: classy-org-openapi.yml
  format: yaml
  label: Classy Fundraising Teams API
  slug: classy-org-fundraising-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/classy-org/refs/heads/main/openapi/classy-org-openapi.yml
- filename: classy-org-openapi.yml
  format: yaml
  label: Classy Transactions API
  slug: classy-org-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/classy-org/refs/heads/main/openapi/classy-org-openapi.yml
- filename: classy-org-openapi.yml
  format: yaml
  label: Classy Recurring Donation Plans API
  slug: classy-org-recurring-donation-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/classy-org/refs/heads/main/openapi/classy-org-openapi.yml
- filename: classy-org-openapi.yml
  format: yaml
  label: Classy Members API
  slug: classy-org-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/classy-org/refs/heads/main/openapi/classy-org-openapi.yml
- filename: classy-org-openapi.yml
  format: yaml
  label: Classy Supporters API
  slug: classy-org-supporters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/classy-org/refs/heads/main/openapi/classy-org-openapi.yml
- filename: classy-org-openapi.yml
  format: yaml
  label: Classy Designations API
  slug: classy-org-designations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/classy-org/refs/heads/main/openapi/classy-org-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: classy.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gofundme.com
  spf: true
hosts:
- cert_expires: Aug 14 03:44:21 2026 GMT
  host: www.classy.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 23:59:59 2026 GMT
  host: developers.gofundme.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 03:44:21 2026 GMT
  host: api.classy.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Classy Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Classy, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Classy
provider_slug: classy-org
slug: classy-org-domain-security
source_filename: classy-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.classy.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 03:44:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.gofundme.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.classy.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 03:44:21 2026 GMT\n  hsts: null\ndomains:\n- domain: classy.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: gofundme.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/classy-org/refs/heads/main/security/classy-org-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Nonprofit
- Fundraising
- Donations
- Peer to Peer
- Philanthropy
- Payments
- GoFundMe Pro
---
