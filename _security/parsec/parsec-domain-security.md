---
api_specs:
- filename: parsec-app-rule-api-openapi.yml
  format: yaml
  label: Parsec App Rule API
  slug: parsec-app-rule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parsec/refs/heads/main/openapi/parsec-app-rule-api-openapi.yml
- filename: parsec-audit-log-api-openapi.yml
  format: yaml
  label: Parsec Audit Log API
  slug: parsec-audit-log-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parsec/refs/heads/main/openapi/parsec-audit-log-api-openapi.yml
- filename: parsec-group-api-openapi.yml
  format: yaml
  label: Parsec Group API
  slug: parsec-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parsec/refs/heads/main/openapi/parsec-group-api-openapi.yml
- filename: parsec-guest-access-invite-api-openapi.yml
  format: yaml
  label: Parsec Guest Access Invite API
  slug: parsec-guest-access-invite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parsec/refs/heads/main/openapi/parsec-guest-access-invite-api-openapi.yml
- filename: parsec-machine-api-openapi.yml
  format: yaml
  label: Parsec Machine API
  slug: parsec-machine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parsec/refs/heads/main/openapi/parsec-machine-api-openapi.yml
- filename: parsec-member-api-openapi.yml
  format: yaml
  label: Parsec Member API
  slug: parsec-member-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parsec/refs/heads/main/openapi/parsec-member-api-openapi.yml
- filename: parsec-member-invite-api-openapi.yml
  format: yaml
  label: Parsec Member Invite API
  slug: parsec-member-invite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parsec/refs/heads/main/openapi/parsec-member-invite-api-openapi.yml
- filename: parsec-relay-api-openapi.yml
  format: yaml
  label: Parsec Relay API
  slug: parsec-relay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parsec/refs/heads/main/openapi/parsec-relay-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: parsec.app
  spf: true
hosts:
- cert_expires: Sep 15 04:04:51 2026 GMT
  host: api.parsec.app
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Parsec Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Parsec, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Parsec
provider_slug: parsec
slug: parsec-domain-security
source_filename: parsec-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.parsec.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 04:04:51 2026 GMT\n  hsts: null\ndomains:\n- domain: parsec.app\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parsec/refs/heads/main/security/parsec-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Remote Desktop
- Cloud Gaming
- Streaming
- Virtual Desktop
- Team Management
- Developer Tools
- Gaming
---
