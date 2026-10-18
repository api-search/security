---
api_specs:
- filename: notarize-cost-centers-api-openapi.yml
  format: yaml
  label: Notarize Cost Centers API
  slug: notarize-cost-centers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-cost-centers-api-openapi.yml
- filename: notarize-documents-api-openapi.yml
  format: yaml
  label: Notarize Documents API
  slug: notarize-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-documents-api-openapi.yml
- filename: notarize-eligibilities-api-openapi.yml
  format: yaml
  label: Notarize Eligibilities API
  slug: notarize-eligibilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-eligibilities-api-openapi.yml
- filename: notarize-enote-api-openapi.yml
  format: yaml
  label: Notarize E Note API
  slug: notarize-enote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-enote-api-openapi.yml
- filename: notarize-integrations-api-openapi.yml
  format: yaml
  label: Notarize Integrations API
  slug: notarize-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-integrations-api-openapi.yml
- filename: notarize-notaries-api-openapi.yml
  format: yaml
  label: Notarize Notaries API
  slug: notarize-notaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-notaries-api-openapi.yml
- filename: notarize-notarization-records-api-openapi.yml
  format: yaml
  label: Notarize Notarization Records API
  slug: notarize-notarization-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-notarization-records-api-openapi.yml
- filename: notarize-oauth-2-0-api-openapi.yml
  format: yaml
  label: Notarize OAuth 2.0 API
  slug: notarize-oauth-2-0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-oauth-2-0-api-openapi.yml
- filename: notarize-oid4vp-api-openapi.yml
  format: yaml
  label: Notarize OID4VP API
  slug: notarize-oid4vp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-oid4vp-api-openapi.yml
- filename: notarize-organizations-api-openapi.yml
  format: yaml
  label: Notarize Organizations API
  slug: notarize-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-organizations-api-openapi.yml
- filename: notarize-referrals-api-openapi.yml
  format: yaml
  label: Notarize Referrals API
  slug: notarize-referrals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-referrals-api-openapi.yml
- filename: notarize-scim-api-openapi.yml
  format: yaml
  label: Notarize SCIM API
  slug: notarize-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-scim-api-openapi.yml
- filename: notarize-security-events-api-openapi.yml
  format: yaml
  label: Notarize Security Events API
  slug: notarize-security-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-security-events-api-openapi.yml
- filename: notarize-templates-api-openapi.yml
  format: yaml
  label: Notarize Templates API
  slug: notarize-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-templates-api-openapi.yml
- filename: notarize-title-agencies-api-openapi.yml
  format: yaml
  label: Notarize Title Agencies API
  slug: notarize-title-agencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-title-agencies-api-openapi.yml
- filename: notarize-transactions-api-openapi.yml
  format: yaml
  label: Notarize Transactions API
  slug: notarize-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-transactions-api-openapi.yml
- filename: notarize-webhooks-api-openapi.yml
  format: yaml
  label: Notarize Webhooks API
  slug: notarize-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: proof.com
  spf: true
hosts:
- cert_expires: Sep 30 04:18:45 2026 GMT
  host: www.proof.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 22 09:25:07 2026 GMT
  host: dev.proof.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: api.proof.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Notarize Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Notarize, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Notarize
provider_slug: notarize
slug: notarize-domain-security
source_filename: notarize-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.proof.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 30 04:18:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dev.proof.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 22 09:25:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.proof.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: proof.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/security/notarize-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Company
- PropTech
- Notarization
- Remote Online Notarization
- Identity Verification
- E-Signature
- Digital Credentials
- Real Estate
- Mortgage
- Legal Tech
---
