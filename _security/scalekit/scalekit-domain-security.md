---
api_specs:
- filename: scalekit-openapi.yml
  format: yaml
  label: Scalekit SSO Connections API
  slug: scalekit-sso-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalekit/refs/heads/main/openapi/scalekit-openapi.yml
- filename: scalekit-openapi.yml
  format: yaml
  label: Scalekit Organizations API
  slug: scalekit-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalekit/refs/heads/main/openapi/scalekit-openapi.yml
- filename: scalekit-openapi.yml
  format: yaml
  label: Scalekit Directory / SCIM API
  slug: scalekit-directory-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalekit/refs/heads/main/openapi/scalekit-openapi.yml
- filename: scalekit-openapi.yml
  format: yaml
  label: Scalekit Users & Memberships API
  slug: scalekit-users-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalekit/refs/heads/main/openapi/scalekit-openapi.yml
- filename: scalekit-openapi.yml
  format: yaml
  label: Scalekit Agent / M2M Auth API
  slug: scalekit-agent-m2m-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalekit/refs/heads/main/openapi/scalekit-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 iodef "mailto:support@scalekit.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: scalekit.com
  spf: true
hosts:
- cert_expires: Sep 30 20:50:33 2026 GMT
  host: www.scalekit.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 23:53:55 2026 GMT
  host: docs.scalekit.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scalekit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scalekit, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Scalekit
provider_slug: scalekit
slug: scalekit-domain-security
source_filename: scalekit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.scalekit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 20:50:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.scalekit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 23:53:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: scalekit.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 iodef \"mailto:support@scalekit.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scalekit/refs/heads/main/security/scalekit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Authentication
- SSO
- SCIM
- Identity
- B2B SaaS
- Agent Auth
---
