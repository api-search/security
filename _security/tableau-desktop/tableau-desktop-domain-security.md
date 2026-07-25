---
api_specs:
- filename: tableau-desktop-authentication-api-openapi.yml
  format: yaml
  label: Tableau Desktop Authentication API
  slug: tableau-desktop-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableau-desktop/refs/heads/main/openapi/tableau-desktop-authentication-api-openapi.yml
- filename: tableau-desktop-data-sources-api-openapi.yml
  format: yaml
  label: Tableau Desktop Data Sources API
  slug: tableau-desktop-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableau-desktop/refs/heads/main/openapi/tableau-desktop-data-sources-api-openapi.yml
- filename: tableau-desktop-projects-api-openapi.yml
  format: yaml
  label: Tableau Desktop Projects API
  slug: tableau-desktop-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableau-desktop/refs/heads/main/openapi/tableau-desktop-projects-api-openapi.yml
- filename: tableau-desktop-server-api-openapi.yml
  format: yaml
  label: Tableau Desktop Server API
  slug: tableau-desktop-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableau-desktop/refs/heads/main/openapi/tableau-desktop-server-api-openapi.yml
- filename: tableau-desktop-sites-api-openapi.yml
  format: yaml
  label: Tableau Desktop Sites API
  slug: tableau-desktop-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableau-desktop/refs/heads/main/openapi/tableau-desktop-sites-api-openapi.yml
- filename: tableau-desktop-users-api-openapi.yml
  format: yaml
  label: Tableau Desktop Users API
  slug: tableau-desktop-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableau-desktop/refs/heads/main/openapi/tableau-desktop-users-api-openapi.yml
- filename: tableau-desktop-workbooks-api-openapi.yml
  format: yaml
  label: Tableau Desktop Workbooks API
  slug: tableau-desktop-workbooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableau-desktop/refs/heads/main/openapi/tableau-desktop-workbooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tableau.com
  spf: true
hosts:
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: www.tableau.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 29 23:59:59 2026 GMT
  host: help.tableau.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tableau Desktop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tableau Desktop, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tableau Desktop
provider_slug: tableau-desktop
slug: tableau-desktop-domain-security
source_filename: tableau-desktop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tableau.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: null\n- host: help.tableau.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tableau.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tableau-desktop/refs/heads/main/security/tableau-desktop-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Business Intelligence
- Data Visualization
- Desktop Application
---
