---
api_specs:
- filename: akuity-apikeyservice-api-openapi.yml
  format: yaml
  label: Akuity API Key Service API
  slug: akuity-apikeyservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akuity/refs/heads/main/openapi/akuity-apikeyservice-api-openapi.yml
- filename: akuity-argocdservice-api-openapi.yml
  format: yaml
  label: Akuity Argo CD Service API
  slug: akuity-argocdservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akuity/refs/heads/main/openapi/akuity-argocdservice-api-openapi.yml
- filename: akuity-authservice-api-openapi.yml
  format: yaml
  label: Akuity Auth Service API
  slug: akuity-authservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akuity/refs/heads/main/openapi/akuity-authservice-api-openapi.yml
- filename: akuity-customroleservice-api-openapi.yml
  format: yaml
  label: Akuity Custom Role Service API
  slug: akuity-customroleservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akuity/refs/heads/main/openapi/akuity-customroleservice-api-openapi.yml
- filename: akuity-extensionservice-api-openapi.yml
  format: yaml
  label: Akuity Extension Service API
  slug: akuity-extensionservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akuity/refs/heads/main/openapi/akuity-extensionservice-api-openapi.yml
- filename: akuity-kargoservice-api-openapi.yml
  format: yaml
  label: Akuity Kargo Service API
  slug: akuity-kargoservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akuity/refs/heads/main/openapi/akuity-kargoservice-api-openapi.yml
- filename: akuity-organizationservice-api-openapi.yml
  format: yaml
  label: Akuity Organization Service API
  slug: akuity-organizationservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akuity/refs/heads/main/openapi/akuity-organizationservice-api-openapi.yml
- filename: akuity-systemservice-api-openapi.yml
  format: yaml
  label: Akuity System Service API
  slug: akuity-systemservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akuity/refs/heads/main/openapi/akuity-systemservice-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: akuity.io
  spf: true
- caa:
  - 0 iodef "mailto:security+ssl@akuity.io"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: akuity.cloud
  spf: true
hosts:
- cert_expires: Oct 28 15:03:44 2026 GMT
  host: akuity.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: docs.akuity.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 20:48:14 2026 GMT
  host: akuity.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Akuity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Akuity, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Akuity
provider_slug: akuity
slug: akuity-domain-security
source_filename: akuity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: akuity.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 15:03:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.akuity.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: akuity.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 20:48:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: akuity.io\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: akuity.cloud\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:security+ssl@akuity.io\"\n  - 0\
  \ issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akuity/refs/heads/main/security/akuity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- GitOps
- Continuous Delivery
- Kubernetes
- Argo CD
- Kargo
- Platform Engineering
- DevOps
- Progressive Delivery
- Cloud Native
- AIOps
- Developer Tools
---
