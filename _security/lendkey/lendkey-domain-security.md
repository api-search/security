---
api_specs:
- filename: lendkey-application-contracts-api-openapi.yml
  format: yaml
  label: LendKey Application Contracts API
  slug: lendkey-application-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-application-contracts-api-openapi.yml
- filename: lendkey-applications-api-openapi.yml
  format: yaml
  label: LendKey applications API
  slug: lendkey-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-applications-api-openapi.yml
- filename: lendkey-auth-api-openapi.yml
  format: yaml
  label: LendKey auth API
  slug: lendkey-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-auth-api-openapi.yml
- filename: lendkey-authentication-api-openapi.yml
  format: yaml
  label: LendKey Authentication API
  slug: lendkey-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-authentication-api-openapi.yml
- filename: lendkey-credit-risk-api-openapi.yml
  format: yaml
  label: LendKey Credit Risk API
  slug: lendkey-credit-risk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-credit-risk-api-openapi.yml
- filename: lendkey-disbursements-api-openapi.yml
  format: yaml
  label: LendKey Disbursements API
  slug: lendkey-disbursements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-disbursements-api-openapi.yml
- filename: lendkey-email-api-openapi.yml
  format: yaml
  label: LendKey email API
  slug: lendkey-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-email-api-openapi.yml
- filename: lendkey-internal-api-openapi.yml
  format: yaml
  label: LendKey internal API
  slug: lendkey-internal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-internal-api-openapi.yml
- filename: lendkey-leads-api-openapi.yml
  format: yaml
  label: LendKey leads API
  slug: lendkey-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-leads-api-openapi.yml
- filename: lendkey-ledger-management-api-openapi.yml
  format: yaml
  label: LendKey Ledger Management API
  slug: lendkey-ledger-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-ledger-management-api-openapi.yml
- filename: lendkey-lender-templates-api-openapi.yml
  format: yaml
  label: LendKey Lender Templates API
  slug: lendkey-lender-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-lender-templates-api-openapi.yml
- filename: lendkey-loans-api-openapi.yml
  format: yaml
  label: LendKey Loans API
  slug: lendkey-loans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-loans-api-openapi.yml
- filename: lendkey-onboarding-api-openapi.yml
  format: yaml
  label: LendKey onboarding API
  slug: lendkey-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-onboarding-api-openapi.yml
- filename: lendkey-payments-api-openapi.yml
  format: yaml
  label: LendKey Payments API
  slug: lendkey-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-payments-api-openapi.yml
- filename: lendkey-webhooks-api-openapi.yml
  format: yaml
  label: LendKey Webhooks API
  slug: lendkey-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "ssladmin.microsoft.com"
  - 0 issue "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "docusign.fr"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lendkey.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: lkeyprod.com
  spf: false
hosts:
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: www.lendkey.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 09:00:03 2026 GMT
  host: api.lendkey.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: proxy.kong.lkeyprod.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Lendkey Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LendKey, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LendKey
provider_slug: lendkey
slug: lendkey-domain-security
source_filename: lendkey-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lendkey.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.lendkey.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 09:00:03 2026 GMT\n  hsts: null\n- host: proxy.kong.lkeyprod.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: lendkey.com\n  dnssec: false\n  caa:\n  - 0 issue \"ssladmin.microsoft.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"docusign.fr\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: lkeyprod.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/security/lendkey-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Lending
- Loans
- Student Loans
- Credit Unions
- Banking
- Loan Origination
- Financial-Services
- Payments
- E-Signature
- Treasury
---
