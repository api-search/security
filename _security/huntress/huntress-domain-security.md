---
api_specs:
- filename: huntress-accounts-api-openapi.yml
  format: yaml
  label: Huntress Accounts API
  slug: huntress-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-accounts-api-openapi.yml
- filename: huntress-actor-api-openapi.yml
  format: yaml
  label: Huntress Actor API
  slug: huntress-actor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-actor-api-openapi.yml
- filename: huntress-agents-api-openapi.yml
  format: yaml
  label: Huntress Agents API
  slug: huntress-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-agents-api-openapi.yml
- filename: huntress-escalations-api-openapi.yml
  format: yaml
  label: Huntress Escalations API
  slug: huntress-escalations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-escalations-api-openapi.yml
- filename: huntress-external-recon-api-openapi.yml
  format: yaml
  label: Huntress External Recon API
  slug: huntress-external-recon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-external-recon-api-openapi.yml
- filename: huntress-identities-api-openapi.yml
  format: yaml
  label: Huntress Identities API
  slug: huntress-identities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-identities-api-openapi.yml
- filename: huntress-incident-reports-api-openapi.yml
  format: yaml
  label: Huntress Incident Reports API
  slug: huntress-incident-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-incident-reports-api-openapi.yml
- filename: huntress-invoices-api-openapi.yml
  format: yaml
  label: Huntress Invoices API
  slug: huntress-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-invoices-api-openapi.yml
- filename: huntress-known-vpns-api-openapi.yml
  format: yaml
  label: Huntress Known VPNs API
  slug: huntress-known-vpns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-known-vpns-api-openapi.yml
- filename: huntress-organizations-api-openapi.yml
  format: yaml
  label: Huntress Organizations API
  slug: huntress-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-organizations-api-openapi.yml
- filename: huntress-platform-actions-api-openapi.yml
  format: yaml
  label: Huntress Platform Actions API
  slug: huntress-platform-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-platform-actions-api-openapi.yml
- filename: huntress-reseller-api-openapi.yml
  format: yaml
  label: Huntress Reseller API
  slug: huntress-reseller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-reseller-api-openapi.yml
- filename: huntress-siem-api-openapi.yml
  format: yaml
  label: Huntress SIEM API
  slug: huntress-siem-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-siem-api-openapi.yml
- filename: huntress-signals-api-openapi.yml
  format: yaml
  label: Huntress Signals API
  slug: huntress-signals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-signals-api-openapi.yml
- filename: huntress-summary-reports-api-openapi.yml
  format: yaml
  label: Huntress Summary Reports API
  slug: huntress-summary-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-summary-reports-api-openapi.yml
- filename: huntress-unwanted-access-rules-api-openapi.yml
  format: yaml
  label: Huntress Unwanted Access Rules API
  slug: huntress-unwanted-access-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-unwanted-access-rules-api-openapi.yml
- filename: huntress-users-api-openapi.yml
  format: yaml
  label: Huntress Users API
  slug: huntress-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: huntress.com
  spf: true
- caa:
  - 0 issuewild "digicert.com"
  - 0 iodef "mailto:security@huntress.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: huntress.io
  spf: true
hosts:
- cert_expires: Jan 27 23:59:59 2027 GMT
  host: www.huntress.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 28 23:59:59 2027 GMT
  host: api.huntress.io
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Huntress Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Huntress, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Huntress
provider_slug: huntress
slug: huntress-domain-security
source_filename: huntress-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.huntress.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.huntress.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: huntress.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: huntress.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 iodef \"mailto:security@huntress.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/security/huntress-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Security
- Cybersecurity
- Managed Detection and Response
- Endpoint Security
- SOC
- SIEM
- Identity Threat Detection
- MSP
- Webhooks
---
