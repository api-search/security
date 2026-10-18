---
api_specs:
- filename: rollee-accounts-api-openapi.yml
  format: yaml
  label: Rollee Accounts API
  slug: rollee-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rollee/refs/heads/main/openapi/rollee-accounts-api-openapi.yml
- filename: rollee-authentication-api-openapi.yml
  format: yaml
  label: Rollee Authentication API
  slug: rollee-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rollee/refs/heads/main/openapi/rollee-authentication-api-openapi.yml
- filename: rollee-companies-api-openapi.yml
  format: yaml
  label: Rollee Companies API
  slug: rollee-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rollee/refs/heads/main/openapi/rollee-companies-api-openapi.yml
- filename: rollee-company-accounts-api-openapi.yml
  format: yaml
  label: Rollee Company accounts API
  slug: rollee-company-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rollee/refs/heads/main/openapi/rollee-company-accounts-api-openapi.yml
- filename: rollee-data-settings-api-openapi.yml
  format: yaml
  label: Rollee Data settings API
  slug: rollee-data-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rollee/refs/heads/main/openapi/rollee-data-settings-api-openapi.yml
- filename: rollee-data-sources-api-openapi.yml
  format: yaml
  label: Rollee Data sources API
  slug: rollee-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rollee/refs/heads/main/openapi/rollee-data-sources-api-openapi.yml
- filename: rollee-employer-endpoints-api-openapi.yml
  format: yaml
  label: Rollee Employer endpoints API
  slug: rollee-employer-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rollee/refs/heads/main/openapi/rollee-employer-endpoints-api-openapi.yml
- filename: rollee-endpoints-api-openapi.yml
  format: yaml
  label: Rollee Endpoints API
  slug: rollee-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rollee/refs/heads/main/openapi/rollee-endpoints-api-openapi.yml
- filename: rollee-fleet-endpoints-api-openapi.yml
  format: yaml
  label: Rollee Fleet endpoints API
  slug: rollee-fleet-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rollee/refs/heads/main/openapi/rollee-fleet-endpoints-api-openapi.yml
- filename: rollee-sessions-api-openapi.yml
  format: yaml
  label: Rollee Sessions API
  slug: rollee-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rollee/refs/heads/main/openapi/rollee-sessions-api-openapi.yml
- filename: rollee-users-api-openapi.yml
  format: yaml
  label: Rollee Users API
  slug: rollee-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rollee/refs/heads/main/openapi/rollee-users-api-openapi.yml
- filename: rollee-webhooks-api-openapi.yml
  format: yaml
  label: Rollee Webhooks API
  slug: rollee-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rollee/refs/heads/main/openapi/rollee-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "zerossl.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: getrollee.com
  spf: true
hosts:
- cert_expires: Oct  6 09:53:49 2026 GMT
  host: www.getrollee.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 00:04:23 2026 GMT
  host: developers.getrollee.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 08:51:18 2026 GMT
  host: api.getrollee.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Rollee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rollee, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Rollee
provider_slug: rollee
slug: rollee-domain-security
source_filename: rollee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getrollee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 09:53:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.getrollee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 00:04:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.getrollee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 08:51:18 2026 GMT\n  hsts: null\ndomains:\n- domain: getrollee.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"zerossl.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rollee/refs/heads/main/security/rollee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Open Finance
- Income Verification
- Employment Verification
- Payroll Data
- Gig Economy
- Alternative Data
- Underwriting
- Lending
- Fintech
---
