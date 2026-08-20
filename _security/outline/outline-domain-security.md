---
api_specs:
- filename: outline-accessrequests-api-openapi.yml
  format: yaml
  label: Outline AccessRequests API
  slug: outline-accessrequests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-accessrequests-api-openapi.yml
- filename: outline-attachments-api-openapi.yml
  format: yaml
  label: Outline Attachments API
  slug: outline-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-attachments-api-openapi.yml
- filename: outline-auth-api-openapi.yml
  format: yaml
  label: Outline Auth API
  slug: outline-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-auth-api-openapi.yml
- filename: outline-collections-api-openapi.yml
  format: yaml
  label: Outline Collections API
  slug: outline-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-collections-api-openapi.yml
- filename: outline-comments-api-openapi.yml
  format: yaml
  label: Outline Comments API
  slug: outline-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-comments-api-openapi.yml
- filename: outline-dataattributes-api-openapi.yml
  format: yaml
  label: Outline DataAttributes API
  slug: outline-dataattributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-dataattributes-api-openapi.yml
- filename: outline-documents-api-openapi.yml
  format: yaml
  label: Outline Documents API
  slug: outline-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-documents-api-openapi.yml
- filename: outline-events-api-openapi.yml
  format: yaml
  label: Outline Events API
  slug: outline-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-events-api-openapi.yml
- filename: outline-fileoperations-api-openapi.yml
  format: yaml
  label: Outline FileOperations API
  slug: outline-fileoperations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-fileoperations-api-openapi.yml
- filename: outline-groups-api-openapi.yml
  format: yaml
  label: Outline Groups API
  slug: outline-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-groups-api-openapi.yml
- filename: outline-oauthauthentications-api-openapi.yml
  format: yaml
  label: Outline OAuthAuthentications API
  slug: outline-oauthauthentications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-oauthauthentications-api-openapi.yml
- filename: outline-oauthclients-api-openapi.yml
  format: yaml
  label: Outline OAuthClients API
  slug: outline-oauthclients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-oauthclients-api-openapi.yml
- filename: outline-revisions-api-openapi.yml
  format: yaml
  label: Outline Revisions API
  slug: outline-revisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-revisions-api-openapi.yml
- filename: outline-shares-api-openapi.yml
  format: yaml
  label: Outline Shares API
  slug: outline-shares-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-shares-api-openapi.yml
- filename: outline-stars-api-openapi.yml
  format: yaml
  label: Outline Stars API
  slug: outline-stars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-stars-api-openapi.yml
- filename: outline-templates-api-openapi.yml
  format: yaml
  label: Outline Templates API
  slug: outline-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-templates-api-openapi.yml
- filename: outline-users-api-openapi.yml
  format: yaml
  label: Outline Users API
  slug: outline-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-users-api-openapi.yml
- filename: outline-views-api-openapi.yml
  format: yaml
  label: Outline Views API
  slug: outline-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-views-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: getoutline.com
  spf: true
hosts:
- cert_expires: Sep 23 17:17:14 2026 GMT
  host: www.getoutline.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 19:02:35 2026 GMT
  host: app.getoutline.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Outline Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Outline, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Outline
provider_slug: outline
slug: outline-domain-security
source_filename: outline-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getoutline.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 17:17:14 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: app.getoutline.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 19:02:35 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: getoutline.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/security/outline-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Knowledge Base
- Wiki
- Documents
- Collaboration
- Open-Source
- Team
---
