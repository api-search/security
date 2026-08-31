---
api_specs:
- filename: strivacity-admin-portal-openapi.yml
  format: yaml
  label: Strivacity Admin API
  slug: strivacity-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/strivacity/refs/heads/main/openapi/strivacity-admin-portal-openapi.yml
- filename: strivacity-myaccount-portal-openapi.yml
  format: yaml
  label: Strivacity MyAccount API
  slug: strivacity-myaccount-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/strivacity/refs/heads/main/openapi/strivacity-myaccount-portal-openapi.yml
- filename: strivacity-native-journey-openapi.yml
  format: yaml
  label: Strivacity Journey Flow API
  slug: strivacity-journey-flow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/strivacity/refs/heads/main/openapi/strivacity-native-journey-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: strivacity.com
  spf: true
hosts:
- cert_expires: Nov 26 22:30:18 2026 GMT
  host: www.strivacity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 23:48:08 2026 GMT
  host: docs.strivacity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Strivacity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Strivacity, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Strivacity
provider_slug: strivacity
slug: strivacity-domain-security
source_filename: strivacity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.strivacity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 22:30:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.strivacity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:48:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: strivacity.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/strivacity/refs/heads/main/security/strivacity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Identity
- customer-identity-and-access-management
- ciam
- Authentication
- Authorization
- openid-connect
- consent-management
- multi-factor-authentication
- Identity Verification
- fraud-detection
- agentic-identity
- Security
---
