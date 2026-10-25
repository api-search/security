---
api_specs:
- filename: idme-applications-openapi-generated.yml
  format: yaml
  label: ID.me applications API
  slug: applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idme/refs/heads/main/openapi/_ae-authored/idme-applications-openapi-generated.yml
- filename: idme-core-openapi-generated.yml
  format: yaml
  label: ID.me core API
  slug: core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idme/refs/heads/main/openapi/_ae-authored/idme-core-openapi-generated.yml
- filename: idme-document-passback-openapi-generated.yml
  format: yaml
  label: ID.me document passback API
  slug: document-passback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idme/refs/heads/main/openapi/_ae-authored/idme-document-passback-openapi-generated.yml
- filename: idme-services-openapi-generated.yml
  format: yaml
  label: ID.me services API
  slug: services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idme/refs/heads/main/openapi/_ae-authored/idme-services-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org; cansignhttpexchanges=yes"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "amazon.com; cansignhttpexchanges=yes"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: id.me
  spf: true
hosts:
- cert_expires: Feb 26 23:59:59 2027 GMT
  host: www.id.me
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  7 08:15:20 2027 GMT
  host: docs.id.me
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 21 23:59:59 2027 GMT
  host: api.id.me
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Idme Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ID.me, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: ID.me
provider_slug: idme
slug: idme-domain-security
source_filename: idme-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.id.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 26 23:59:59 2027 GMT\n  hsts: null\n- host: docs.id.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 08:15:20 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.id.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: id.me\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org; cansignhttpexchanges=yes\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"amazon.com; cansignhttpexchanges=yes\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/idme/refs/heads/main/security/idme-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Identity
- Identity Verification
- Authentication
- OpenID Connect
- SAML
- SSO
- Digital Identity
- KYC
- Fraud Prevention
- Government
- Identity Federation
---
