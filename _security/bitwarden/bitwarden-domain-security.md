---
api_specs:
- filename: bitwarden-public-swagger.json
  format: json
  label: Bitwarden Public API - Members
  slug: public-members
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitwarden/refs/heads/main/openapi/bitwarden-public-swagger.json
- filename: bitwarden-public-swagger.json
  format: json
  label: Bitwarden Public API - Groups
  slug: public-groups
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitwarden/refs/heads/main/openapi/bitwarden-public-swagger.json
- filename: bitwarden-public-swagger.json
  format: json
  label: Bitwarden Public API - Collections
  slug: public-collections
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitwarden/refs/heads/main/openapi/bitwarden-public-swagger.json
- filename: bitwarden-public-swagger.json
  format: json
  label: Bitwarden Public API - Policies
  slug: public-policies
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitwarden/refs/heads/main/openapi/bitwarden-public-swagger.json
- filename: bitwarden-public-swagger.json
  format: json
  label: Bitwarden Public API - Event Logs
  slug: public-events
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitwarden/refs/heads/main/openapi/bitwarden-public-swagger.json
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: bitwarden.com
  spf: true
hosts:
- cert_expires: Oct  7 04:13:13 2026 GMT
  host: bitwarden.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 07:43:09 2026 GMT
  host: api.bitwarden.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 07:33:28 2026 GMT
  host: identity.bitwarden.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bitwarden Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bitwarden, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Bitwarden
provider_slug: bitwarden
slug: bitwarden-domain-security
source_filename: bitwarden-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bitwarden.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 04:13:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: api.bitwarden.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 07:43:09 2026 GMT\n  hsts: null\n- host: identity.bitwarden.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 07:33:28 2026 GMT\n  hsts: null\ndomains:\n- domain: bitwarden.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitwarden/refs/heads/main/security/bitwarden-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Security
- Password Manager
- Open Source
- Vault
- Identity
- SCIM
---
