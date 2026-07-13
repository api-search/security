---
api_specs:
- filename: quickbooks-online-webhooks-asyncapi.yml
  format: yaml
  label: QuickBooks Online Accounting API
  slug: online-accounting
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/quickbooks/refs/heads/main/asyncapi/quickbooks-online-webhooks-asyncapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:Tech-PINetworkServiceOperations@intuit.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: intuit.com
  spf: true
hosts:
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: quickbooks.intuit.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: developer.intuit.com
  https: false
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: quickbooks.api.intuit.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Quickbooks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for QuickBooks, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: QuickBooks
provider_slug: quickbooks
slug: quickbooks-domain-security
source_filename: quickbooks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quickbooks.intuit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: null\n- host: developer.intuit.com\n  https: false\n- host: quickbooks.api.intuit.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: intuit.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:Tech-PINetworkServiceOperations@intuit.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quickbooks/refs/heads/main/security/quickbooks-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Accounting
- Bookkeeping
- Small Business
- Financials
- Invoicing
- Payroll
- Tax
---
