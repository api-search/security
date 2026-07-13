---
api_specs:
- filename: open-api-spec.yaml
  format: yaml
  label: WorkOS API
  slug: workos
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/workos/openapi-spec/main/spec/open-api-spec.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: workos.com
  spf: true
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: workos-test.com
  spf: true
hosts:
- cert_expires: Sep  2 19:29:52 2026 GMT
  host: workos.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 07:11:00 2026 GMT
  host: api.workos.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 10:20:32 2026 GMT
  host: api.workos-test.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Workos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WorkOS, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: WorkOS
provider_slug: workos
slug: workos-domain-security
source_filename: workos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: workos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 19:29:52 2026 GMT\n  hsts: false\n- host: api.workos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 07:11:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.workos-test.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 10:20:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: workos.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: workos-test.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy:\
  \ none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workos/refs/heads/main/security/workos-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Authentication
- Identity Provider
- SSO
- SAML
- OIDC
- SCIM
- Directory Sync
- Authorization
- FGA
- Audit Logs
- MFA
- B2B SaaS
- Agents
- MCP
---
