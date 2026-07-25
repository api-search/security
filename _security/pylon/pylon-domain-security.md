---
api_specs:
- filename: pylon-accounts-api-openapi.yml
  format: yaml
  label: Pylon Accounts API
  slug: pylon-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pylon/refs/heads/main/openapi/pylon-accounts-api-openapi.yml
- filename: pylon-contacts-api-openapi.yml
  format: yaml
  label: Pylon Contacts API
  slug: pylon-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pylon/refs/heads/main/openapi/pylon-contacts-api-openapi.yml
- filename: pylon-custom-fields-api-openapi.yml
  format: yaml
  label: Pylon Custom Fields API
  slug: pylon-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pylon/refs/heads/main/openapi/pylon-custom-fields-api-openapi.yml
- filename: pylon-issues-api-openapi.yml
  format: yaml
  label: Pylon Issues API
  slug: pylon-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pylon/refs/heads/main/openapi/pylon-issues-api-openapi.yml
- filename: pylon-knowledge-base-api-openapi.yml
  format: yaml
  label: Pylon Knowledge Base API
  slug: pylon-knowledge-base-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pylon/refs/heads/main/openapi/pylon-knowledge-base-api-openapi.yml
- filename: pylon-tags-api-openapi.yml
  format: yaml
  label: Pylon Tags API
  slug: pylon-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pylon/refs/heads/main/openapi/pylon-tags-api-openapi.yml
- filename: pylon-tasks-api-openapi.yml
  format: yaml
  label: Pylon Tasks API
  slug: pylon-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pylon/refs/heads/main/openapi/pylon-tasks-api-openapi.yml
- filename: pylon-teams-api-openapi.yml
  format: yaml
  label: Pylon Teams API
  slug: pylon-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pylon/refs/heads/main/openapi/pylon-teams-api-openapi.yml
- filename: pylon-users-api-openapi.yml
  format: yaml
  label: Pylon Users API
  slug: pylon-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pylon/refs/heads/main/openapi/pylon-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issuewild "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: usepylon.com
  spf: true
hosts:
- cert_expires: Sep  5 08:42:09 2026 GMT
  host: usepylon.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 14:14:10 2026 GMT
  host: docs.usepylon.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: api.usepylon.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pylon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pylon, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Pylon
provider_slug: pylon
slug: pylon-domain-security
source_filename: pylon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: usepylon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 08:42:09 2026 GMT\n  hsts: false\n- host: docs.usepylon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 14:14:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.usepylon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: usepylon.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pylon/refs/heads/main/security/pylon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Customer Support
- Customer Operations
- Ticketing
- Knowledge Base
- B2B
- Help Desk
---
