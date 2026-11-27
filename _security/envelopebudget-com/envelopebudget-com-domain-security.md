---
api_specs:
- filename: envelopebudget-com-accounts-api-openapi.yml
  format: yaml
  label: EnvelopeBudget Accounts API
  slug: envelopebudget-com-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/envelopebudget-com/openapi/envelopebudget-com-accounts-api-openapi.yml
- filename: envelopebudget-com-auth-api-openapi.yml
  format: yaml
  label: EnvelopeBudget Auth API
  slug: envelopebudget-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/envelopebudget-com/openapi/envelopebudget-com-auth-api-openapi.yml
- filename: envelopebudget-com-envelopes-api-openapi.yml
  format: yaml
  label: EnvelopeBudget Envelopes API
  slug: envelopebudget-com-envelopes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/envelopebudget-com/openapi/envelopebudget-com-envelopes-api-openapi.yml
- filename: envelopebudget-com-transactions-api-openapi.yml
  format: yaml
  label: EnvelopeBudget Transactions API
  slug: envelopebudget-com-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/envelopebudget-com/openapi/envelopebudget-com-transactions-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: envelopebudget.com
  spf: true
hosts:
- cert_expires: Dec 13 05:20:04 2026 GMT
  host: envelopebudget.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: EnvelopeBudget Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EnvelopeBudget, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: EnvelopeBudget
provider_slug: envelopebudget-com
slug: envelopebudget-com-domain-security
source_filename: envelopebudget-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: envelopebudget.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 05:20:04 2026 GMT\n  hsts: false\ndomains:\n- domain: envelopebudget.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/envelopebudget-com/security/envelopebudget-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Finance
- Budgeting
- Personal Finance
- Couples
- Families
---
