---
api_specs:
- filename: quickbooks-accounting.yml
  format: yaml
  label: QuickBooks Online Accounting API
  slug: quickbooks-accounting
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intuit/refs/heads/main/openapi/quickbooks-accounting.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "globalsign.com"
  - 0 issue "comodoca.com"
  - 0 iodef "mailto:Tech-PINetworkServiceOperations@intuit.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: intuit.com
  spf: true
hosts:
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: developer.intuit.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Intuit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Intuit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Intuit
provider_slug: intuit
slug: intuit-domain-security
source_filename: intuit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.intuit.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: intuit.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 iodef \"mailto:Tech-PINetworkServiceOperations@intuit.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intuit/refs/heads/main/security/intuit-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Accounting
- Custom Fields
- Financial
- Financial Services
- Invoicing
- Payments
- Payroll
- Project Management
- Sales Tax
- Small Business
- Tax
- Tax Preparation
- Taxes
- Time Tracking
- Fortune 1000
---
