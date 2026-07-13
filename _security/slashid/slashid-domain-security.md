---
api_specs:
- filename: slashid-openapi-latest.yaml
  format: yaml
  label: SlashID API
  slug: slashid-api
  spec_type: OpenAPI
  url: https://cdn.slashid.com/slashid-openapi-latest.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: slashid.dev
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: slashid.com
  spf: true
hosts:
- cert_expires: Sep 14 21:11:48 2026 GMT
  host: www.slashid.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: developer.slashid.dev
  https: false
- cert_expires: Sep 23 01:47:38 2026 GMT
  host: api.slashid.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Slashid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SlashID, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SlashID
provider_slug: slashid
slug: slashid-domain-security
source_filename: slashid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.slashid.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 21:11:48 2026 GMT\n  hsts: false\n- host: developer.slashid.dev\n  https: false\n- host: api.slashid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 01:47:38 2026 GMT\n  hsts: null\ndomains:\n- domain: slashid.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: slashid.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/slashid/refs/heads/main/security/slashid-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Identity
- Authentication
- Passwordless
- MFA
- Passkeys
- User Management
- CIAM
- OAuth2
- OIDC
- SSO
- RBAC
- Security
---
