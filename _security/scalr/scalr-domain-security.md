---
api_specs:
- filename: scalr-user-openapi.yml
  format: yaml
  label: Scalr User API
  slug: scalr-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalr/refs/heads/main/openapi/scalr-user-openapi.yml
- filename: scalr-account-openapi.yml
  format: yaml
  label: Scalr Account API
  slug: scalr-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalr/refs/heads/main/openapi/scalr-account-openapi.yml
- filename: scalr-global-openapi.yml
  format: yaml
  label: Scalr Global API
  slug: scalr-global-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalr/refs/heads/main/openapi/scalr-global-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: scalr.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  - 0 issuewild "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "godaddy.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: scalr.io
  spf: true
hosts:
- cert_expires: Oct  8 01:43:20 2026 GMT
  host: scalr.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 01:43:20 2026 GMT
  host: api-explorer.scalr.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 01:17:18 2026 GMT
  host: docs.scalr.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scalr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scalr, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Scalr
provider_slug: scalr
slug: scalr-domain-security
source_filename: scalr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: scalr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 01:43:20 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api-explorer.scalr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 01:43:20 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.scalr.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 01:17:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: scalr.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: scalr.io\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"pki.goog\"\
  \n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scalr/refs/heads/main/security/scalr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- FinOps
- GitOps
- Infrastructure as Code
- Kubernetes
- OPA
- OpenTofu
- Policy
- Terraform
---
