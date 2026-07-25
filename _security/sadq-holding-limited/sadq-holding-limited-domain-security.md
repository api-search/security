---
api_specs:
- filename: sadq-holding-limited-archiving-delegations-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Archiving & Delegations API
  slug: sadq-holding-limited-archiving-delegations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-archiving-delegations-api-openapi.yml
- filename: sadq-holding-limited-authentication-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Authentication API
  slug: sadq-holding-limited-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-authentication-api-openapi.yml
- filename: sadq-holding-limited-configuration-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Configuration API
  slug: sadq-holding-limited-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-configuration-api-openapi.yml
- filename: sadq-holding-limited-documents-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Documents API
  slug: sadq-holding-limited-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-documents-api-openapi.yml
- filename: sadq-holding-limited-envelopes-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Envelopes API
  slug: sadq-holding-limited-envelopes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-envelopes-api-openapi.yml
- filename: sadq-holding-limited-esign-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited eSign API
  slug: sadq-holding-limited-esign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-esign-api-openapi.yml
- filename: sadq-holding-limited-invitations-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Invitations API
  slug: sadq-holding-limited-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-invitations-api-openapi.yml
- filename: sadq-holding-limited-kyb-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited KYB API
  slug: sadq-holding-limited-kyb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-kyb-api-openapi.yml
- filename: sadq-holding-limited-reports-requests-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Reports & Requests API
  slug: sadq-holding-limited-reports-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-reports-requests-api-openapi.yml
- filename: sadq-holding-limited-sign-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Sign API
  slug: sadq-holding-limited-sign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-sign-api-openapi.yml
- filename: sadq-holding-limited-templates-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Templates API
  slug: sadq-holding-limited-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-templates-api-openapi.yml
- filename: sadq-holding-limited-users-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Users API
  slug: sadq-holding-limited-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-users-api-openapi.yml
- filename: sadq-holding-limited-webhooks-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Webhooks API
  slug: sadq-holding-limited-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-webhooks-api-openapi.yml
- filename: sadq-holding-limited-workflows-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Workflows API
  slug: sadq-holding-limited-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-workflows-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issuewild "sectigo.com"
  dmarc: false
  dnssec: false
  domain: sadq-sa.com
  spf: false
- caa:
  - 0 issuewild "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sadq.sa
  spf: true
hosts:
- cert_expires: Feb 26 23:59:59 2027 GMT
  host: sadq-sa.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 26 23:59:59 2027 GMT
  host: api.sadq.sa
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 26 23:59:59 2027 GMT
  host: sandbox-api.sadq-sa.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Sadq Holding Limited Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sadq Holding Limited, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Sadq Holding Limited
provider_slug: sadq-holding-limited
slug: sadq-holding-limited-domain-security
source_filename: sadq-holding-limited-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sadq-sa.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 26 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.sadq.sa\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 26 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sandbox-api.sadq-sa.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 26 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: sadq-sa.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"sectigo.com\"\n  spf: false\n  dmarc: false\n- domain: sadq.sa\n  dnssec: false\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/security/sadq-holding-limited-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- E-Signature
- Digital Signature
- Identity
- KYB
- Document Management
- Saudi Arabia
- Nafath
- Webhooks
- Agent Ready
---
