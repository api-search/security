---
api_specs:
- filename: commareports-com-account-api-openapi.yml
  format: yaml
  label: Comma Account API
  slug: commareports-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commareports-com/openapi/commareports-com-account-api-openapi.yml
- filename: commareports-com-assets-api-openapi.yml
  format: yaml
  label: Comma Assets API
  slug: commareports-com-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commareports-com/openapi/commareports-com-assets-api-openapi.yml
- filename: commareports-com-comments-api-openapi.yml
  format: yaml
  label: Comma Comments API
  slug: commareports-com-comments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commareports-com/openapi/commareports-com-comments-api-openapi.yml
- filename: commareports-com-connectors-api-openapi.yml
  format: yaml
  label: Comma Connectors API
  slug: commareports-com-connectors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commareports-com/openapi/commareports-com-connectors-api-openapi.yml
- filename: commareports-com-meta-api-openapi.yml
  format: yaml
  label: Comma Meta API
  slug: commareports-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commareports-com/openapi/commareports-com-meta-api-openapi.yml
- filename: commareports-com-notifications-api-openapi.yml
  format: yaml
  label: Comma Notifications API
  slug: commareports-com-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commareports-com/openapi/commareports-com-notifications-api-openapi.yml
- filename: commareports-com-reports-api-openapi.yml
  format: yaml
  label: Comma Reports API
  slug: commareports-com-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commareports-com/openapi/commareports-com-reports-api-openapi.yml
- filename: commareports-com-reviewers-api-openapi.yml
  format: yaml
  label: Comma Reviewers API
  slug: commareports-com-reviewers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commareports-com/openapi/commareports-com-reviewers-api-openapi.yml
- filename: commareports-com-reviews-api-openapi.yml
  format: yaml
  label: Comma Reviews API
  slug: commareports-com-reviews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commareports-com/openapi/commareports-com-reviews-api-openapi.yml
- filename: commareports-com-revisions-api-openapi.yml
  format: yaml
  label: Comma Revisions API
  slug: commareports-com-revisions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commareports-com/openapi/commareports-com-revisions-api-openapi.yml
- filename: commareports-com-routines-api-openapi.yml
  format: yaml
  label: Comma Routines API
  slug: commareports-com-routines-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commareports-com/openapi/commareports-com-routines-api-openapi.yml
- filename: commareports-com-sharing-api-openapi.yml
  format: yaml
  label: Comma Sharing API
  slug: commareports-com-sharing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commareports-com/openapi/commareports-com-sharing-api-openapi.yml
- filename: commareports-com-skills-api-openapi.yml
  format: yaml
  label: Comma Skills API
  slug: commareports-com-skills-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commareports-com/openapi/commareports-com-skills-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:info@getnadir.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: commareports.com
  spf: true
hosts:
- cert_expires: Dec 12 03:00:57 2026 GMT
  host: commareports.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Comma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Comma, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Comma
provider_slug: commareports-com
slug: commareports-com-domain-security
source_filename: commareports-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: commareports.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 03:00:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: commareports.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:info@getnadir.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/commareports-com/security/commareports-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Reports
- Collaboration
- Comments
- HTML
- MCP
- AI Agents
- Data Visualization
---
