---
api_specs:
- filename: storecove-additionaltaxidentifiers-api-openapi.yml
  format: yaml
  label: Storecove Additional Tax Identifiers API
  slug: storecove-additionaltaxidentifiers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/storecove/openapi/storecove-additionaltaxidentifiers-api-openapi.yml
- filename: storecove-administrations-api-openapi.yml
  format: yaml
  label: Storecove Administrations API
  slug: storecove-administrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/storecove/openapi/storecove-administrations-api-openapi.yml
- filename: storecove-c5activation-api-openapi.yml
  format: yaml
  label: Storecove C5Activation API
  slug: storecove-c5activation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/storecove/openapi/storecove-c5activation-api-openapi.yml
- filename: storecove-discovery-api-openapi.yml
  format: yaml
  label: Storecove Discovery API
  slug: storecove-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/storecove/openapi/storecove-discovery-api-openapi.yml
- filename: storecove-invoicesubmissions-api-openapi.yml
  format: yaml
  label: Storecove Invoice Submissions API
  slug: storecove-invoicesubmissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/storecove/openapi/storecove-invoicesubmissions-api-openapi.yml
- filename: storecove-legalentities-api-openapi.yml
  format: yaml
  label: Storecove Legal Entities API
  slug: storecove-legalentities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/storecove/openapi/storecove-legalentities-api-openapi.yml
- filename: storecove-peppolidentifiers-api-openapi.yml
  format: yaml
  label: Storecove Peppol Identifiers API
  slug: storecove-peppolidentifiers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/storecove/openapi/storecove-peppolidentifiers-api-openapi.yml
- filename: storecove-purchaseinvoices-api-openapi.yml
  format: yaml
  label: Storecove Purchase Invoices API
  slug: storecove-purchaseinvoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/storecove/openapi/storecove-purchaseinvoices-api-openapi.yml
- filename: storecove-receiveddocuments-api-openapi.yml
  format: yaml
  label: Storecove Received Documents API
  slug: storecove-receiveddocuments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/storecove/openapi/storecove-receiveddocuments-api-openapi.yml
- filename: storecove-webhookinstances-api-openapi.yml
  format: yaml
  label: Storecove Webhook Instances API
  slug: storecove-webhookinstances-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/storecove/openapi/storecove-webhookinstances-api-openapi.yml
- filename: storecove-document-submissions-api-openapi.yml
  format: yaml
  label: Storecove document submissions API
  slug: storecove-document-submissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/storecove/openapi/storecove-document-submissions-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "amazon.com"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: storecove.com
  spf: true
hosts:
- cert_expires: Dec 31 12:44:46 2026 GMT
  host: www.storecove.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Storecove Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Storecove, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Storecove
provider_slug: storecove
slug: storecove-domain-security
source_filename: storecove-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.storecove.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 12:44:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: storecove.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/storecove/security/storecove-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- E-Invoicing
- PEPPOL
- Tax Compliance
- Invoicing
- Accounting
- ERP Integration
- Fintech
---
