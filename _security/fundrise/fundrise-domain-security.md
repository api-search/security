---
api_specs:
- filename: fundrise-acknowledgments-api-openapi.yml
  format: yaml
  label: Fundrise Acknowledgments API
  slug: fundrise-acknowledgments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundrise/refs/heads/main/openapi/fundrise-acknowledgments-api-openapi.yml
- filename: fundrise-authentication-api-openapi.yml
  format: yaml
  label: Fundrise Authentication API
  slug: fundrise-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundrise/refs/heads/main/openapi/fundrise-authentication-api-openapi.yml
- filename: fundrise-clients-api-openapi.yml
  format: yaml
  label: Fundrise Clients API
  slug: fundrise-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundrise/refs/heads/main/openapi/fundrise-clients-api-openapi.yml
- filename: fundrise-holdings-api-openapi.yml
  format: yaml
  label: Fundrise Holdings API
  slug: fundrise-holdings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundrise/refs/heads/main/openapi/fundrise-holdings-api-openapi.yml
- filename: fundrise-investments-api-openapi.yml
  format: yaml
  label: Fundrise Investments API
  slug: fundrise-investments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundrise/refs/heads/main/openapi/fundrise-investments-api-openapi.yml
- filename: fundrise-liquidations-api-openapi.yml
  format: yaml
  label: Fundrise Liquidations API
  slug: fundrise-liquidations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundrise/refs/heads/main/openapi/fundrise-liquidations-api-openapi.yml
- filename: fundrise-offerings-api-openapi.yml
  format: yaml
  label: Fundrise Offerings API
  slug: fundrise-offerings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundrise/refs/heads/main/openapi/fundrise-offerings-api-openapi.yml
- filename: fundrise-tax-forms-api-openapi.yml
  format: yaml
  label: Fundrise Tax Forms API
  slug: fundrise-tax-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundrise/refs/heads/main/openapi/fundrise-tax-forms-api-openapi.yml
- filename: fundrise-transactions-api-openapi.yml
  format: yaml
  label: Fundrise Transactions API
  slug: fundrise-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundrise/refs/heads/main/openapi/fundrise-transactions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: fundrise.com
  spf: true
hosts:
- cert_expires: Oct 12 23:59:59 2026 GMT
  host: fundrise.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: sandbox.fundrise.com
  https: false
kind: domain-security
layout: security
method: probed
name: Fundrise Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fundrise, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Fundrise
provider_slug: fundrise
slug: fundrise-domain-security
source_filename: fundrise-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fundrise.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 23:59:59 2026 GMT\n  hsts: null\n- host: sandbox.fundrise.com\n  https: false\ndomains:\n- domain: fundrise.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fundrise/refs/heads/main/security/fundrise-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Financial Services
- Investing
- Real Estate
- Private Credit
- Venture Capital
- Alternative Assets
- Wealth Management
- Fintech
- Embedded Investing
---
