---
api_specs:
- filename: passage-1password-openapi.yml
  format: yaml
  label: Passage Management API
  slug: passage-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passage-1password/refs/heads/main/openapi/passage-1password-openapi.yml
- filename: passage-1password-openapi.yml
  format: yaml
  label: Passage Users API
  slug: passage-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passage-1password/refs/heads/main/openapi/passage-1password-openapi.yml
- filename: passage-1password-openapi.yml
  format: yaml
  label: Passage Magic Links API
  slug: passage-magic-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passage-1password/refs/heads/main/openapi/passage-1password-openapi.yml
- filename: passage-1password-openapi.yml
  format: yaml
  label: Passage Authentication API
  slug: passage-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passage-1password/refs/heads/main/openapi/passage-1password-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:alerts+caa@agilebits.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 1password.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: passage.id
  spf: false
hosts:
- cert_expires: Mar  6 23:59:59 2027 GMT
  host: passage.1password.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: docs.passage.id
  https: false
- host: api.passage.id
  https: false
kind: domain-security
layout: security
method: probed
name: Passage 1Password Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Passage by 1Password, probed live across 3 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Passage by 1Password
provider_slug: passage-1password
slug: passage-1password-domain-security
source_filename: passage-1password-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: passage.1password.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.passage.id\n  https: false\n- host: api.passage.id\n  https: false\ndomains:\n- domain: 1password.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:alerts+caa@agilebits.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: passage.id\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/passage-1password/refs/heads/main/security/passage-1password-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Authentication
- Passkeys
- WebAuthn
- Passwordless
- Identity
- Magic Links
---
