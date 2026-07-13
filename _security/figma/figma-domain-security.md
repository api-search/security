---
api_specs:
- filename: figma-api-openapi.yml
  format: yaml
  label: Figma API
  slug: figma-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-api-openapi.yml
- filename: figma-rest-api-openapi.yml
  format: yaml
  label: Figma REST API
  slug: figma-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-rest-api-openapi.yml
- filename: figma-files-api-openapi.yml
  format: yaml
  label: Figma Files API
  slug: figma-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-files-api-openapi.yml
- filename: figma-images-api-openapi.yml
  format: yaml
  label: Figma Images API
  slug: figma-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-images-api-openapi.yml
- filename: figma-teams-api-openapi.yml
  format: yaml
  label: Figma Teams API
  slug: figma-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-teams-api-openapi.yml
- filename: figma-projects-api-openapi.yml
  format: yaml
  label: Figma Projects API
  slug: figma-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-projects-api-openapi.yml
- filename: figma-me-api-openapi.yml
  format: yaml
  label: Figma Me API
  slug: figma-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-me-api-openapi.yml
- filename: figma-rest-api-openapi.yml
  format: yaml
  label: Figma Components API
  slug: figma-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-rest-api-openapi.yml
- filename: figma-component-sets-api-openapi.yml
  format: yaml
  label: Figma Component Sets API
  slug: figma-component-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-component-sets-api-openapi.yml
- filename: figma-styles-api-openapi.yml
  format: yaml
  label: Figma Styles API
  slug: figma-styles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-styles-api-openapi.yml
- filename: figma-activity-logs-api-openapi.yml
  format: yaml
  label: Figma Activity Logs API
  slug: figma-activity-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-activity-logs-api-openapi.yml
- filename: figma-payments-api-openapi.yml
  format: yaml
  label: Figma Payments API
  slug: figma-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-payments-api-openapi.yml
- filename: figma-dev-resources-api-openapi.yml
  format: yaml
  label: Figma Dev Resources API
  slug: figma-dev-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-dev-resources-api-openapi.yml
- filename: figma-analytics-api-openapi.yml
  format: yaml
  label: Figma Analytics API
  slug: figma-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-analytics-api-openapi.yml
- filename: figma-rest-api-openapi.yml
  format: yaml
  label: Figma Comments API
  slug: figma-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-rest-api-openapi.yml
- filename: figma-rest-api-openapi.yml
  format: yaml
  label: Figma Version History API
  slug: figma-version-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-rest-api-openapi.yml
- filename: figma-rest-api-openapi.yml
  format: yaml
  label: Figma Variables API
  slug: figma-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-rest-api-openapi.yml
- filename: figma-rest-api-openapi.yml
  format: yaml
  label: Figma Library Analytics API
  slug: figma-library-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-rest-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:security@figma.com"
  - 0 issue "amazonaws.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: figma.com
  spf: true
hosts:
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: www.figma.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: api.figma.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: developers.figma.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Figma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Figma, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Figma
provider_slug: figma
slug: figma-domain-security
source_filename: figma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.figma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.figma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.figma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: figma.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:security@figma.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/security/figma-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
---
