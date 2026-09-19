---
api_specs:
- filename: authologic-aml-api-openapi.yml
  format: yaml
  label: Authologic AML API
  slug: authologic-aml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/openapi/authologic-aml-api-openapi.yml
- filename: authologic-advanced-api-openapi.yml
  format: yaml
  label: Authologic Advanced API
  slug: authologic-advanced-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/openapi/authologic-advanced-api-openapi.yml
- filename: authologic-affordability-assessment-api-openapi.yml
  format: yaml
  label: Authologic Affordability assessment API
  slug: authologic-affordability-assessment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/openapi/authologic-affordability-assessment-api-openapi.yml
- filename: authologic-aml-api-openapi.yml
  format: yaml
  label: Authologic AML API
  slug: authologic-aml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/openapi/authologic-aml-api-openapi.yml
- filename: authologic-bank-api-openapi.yml
  format: yaml
  label: Authologic Bank API
  slug: authologic-bank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/openapi/authologic-bank-api-openapi.yml
- filename: authologic-conversation-api-openapi.yml
  format: yaml
  label: Authologic Conversation API
  slug: authologic-conversation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/openapi/authologic-conversation-api-openapi.yml
- filename: authologic-database-verification-api-openapi.yml
  format: yaml
  label: Authologic Database Verification API
  slug: authologic-database-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/openapi/authologic-database-verification-api-openapi.yml
- filename: authologic-enterprise-integration-api-openapi.yml
  format: yaml
  label: Authologic Enterprise Integration API
  slug: authologic-enterprise-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/openapi/authologic-enterprise-integration-api-openapi.yml
- filename: authologic-metadata-api-openapi.yml
  format: yaml
  label: Authologic Metadata API
  slug: authologic-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/openapi/authologic-metadata-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "certum.pl"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: authologic.com
  spf: true
hosts:
- cert_expires: Nov  6 03:04:53 2026 GMT
  host: authologic.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 12 13:37:49 2026 GMT
  host: developer.authologic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 15:14:19 2026 GMT
  host: api.authologic.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Authologic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Authologic, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Authologic
provider_slug: authologic
slug: authologic-domain-security
source_filename: authologic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: authologic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 03:04:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.authologic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 13:37:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.authologic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 15:14:19 2026 GMT\n  hsts: null\ndomains:\n- domain: authologic.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"certum.pl\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/security/authologic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AML
- Digital Identity
- eID
- Identity Verification
- KYB
- KYC
- Liveness Check
---
