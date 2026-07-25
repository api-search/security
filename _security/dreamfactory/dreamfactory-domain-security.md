---
api_specs:
- filename: dreamfactory-system-api-openapi.yml
  format: yaml
  label: DreamFactory System API
  slug: system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/openapi/dreamfactory-system-api-openapi.yml
- filename: dreamfactory-admin-api-openapi.yml
  format: yaml
  label: DreamFactory Admin API
  slug: dreamfactory-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/openapi/dreamfactory-admin-api-openapi.yml
- filename: dreamfactory-app-api-openapi.yml
  format: yaml
  label: DreamFactory App API
  slug: dreamfactory-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/openapi/dreamfactory-app-api-openapi.yml
- filename: dreamfactory-appgroup-api-openapi.yml
  format: yaml
  label: DreamFactory AppGroup API
  slug: dreamfactory-appgroup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/openapi/dreamfactory-appgroup-api-openapi.yml
- filename: dreamfactory-cors-api-openapi.yml
  format: yaml
  label: DreamFactory CORS API
  slug: dreamfactory-cors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/openapi/dreamfactory-cors-api-openapi.yml
- filename: dreamfactory-custom-api-openapi.yml
  format: yaml
  label: DreamFactory Custom API
  slug: dreamfactory-custom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/openapi/dreamfactory-custom-api-openapi.yml
- filename: dreamfactory-emailtemplate-api-openapi.yml
  format: yaml
  label: DreamFactory EmailTemplate API
  slug: dreamfactory-emailtemplate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/openapi/dreamfactory-emailtemplate-api-openapi.yml
- filename: dreamfactory-environment-api-openapi.yml
  format: yaml
  label: DreamFactory Environment API
  slug: dreamfactory-environment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/openapi/dreamfactory-environment-api-openapi.yml
- filename: dreamfactory-event-api-openapi.yml
  format: yaml
  label: DreamFactory Event API
  slug: dreamfactory-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/openapi/dreamfactory-event-api-openapi.yml
- filename: dreamfactory-limit-api-openapi.yml
  format: yaml
  label: DreamFactory Limit API
  slug: dreamfactory-limit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/openapi/dreamfactory-limit-api-openapi.yml
- filename: dreamfactory-lookup-api-openapi.yml
  format: yaml
  label: DreamFactory Lookup API
  slug: dreamfactory-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/openapi/dreamfactory-lookup-api-openapi.yml
- filename: dreamfactory-package-api-openapi.yml
  format: yaml
  label: DreamFactory Package API
  slug: dreamfactory-package-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/openapi/dreamfactory-package-api-openapi.yml
- filename: dreamfactory-role-api-openapi.yml
  format: yaml
  label: DreamFactory Role API
  slug: dreamfactory-role-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/openapi/dreamfactory-role-api-openapi.yml
- filename: dreamfactory-scripttype-api-openapi.yml
  format: yaml
  label: DreamFactory ScriptType API
  slug: dreamfactory-scripttype-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/openapi/dreamfactory-scripttype-api-openapi.yml
- filename: dreamfactory-servicetype-api-openapi.yml
  format: yaml
  label: DreamFactory ServiceType API
  slug: dreamfactory-servicetype-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/openapi/dreamfactory-servicetype-api-openapi.yml
- filename: dreamfactory-user-api-openapi.yml
  format: yaml
  label: DreamFactory User API
  slug: dreamfactory-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/openapi/dreamfactory-user-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dreamfactory.com
  spf: true
hosts:
- cert_expires: Oct  2 20:59:12 2026 GMT
  host: www.dreamfactory.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 20:31:09 2026 GMT
  host: guide.dreamfactory.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Dreamfactory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DreamFactory, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DreamFactory
provider_slug: dreamfactory
slug: dreamfactory-domain-security
source_filename: dreamfactory-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dreamfactory.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 20:59:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: guide.dreamfactory.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 14 20:31:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dreamfactory.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/security/dreamfactory-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automation
- Deployment
- Documentation
- Generation
- Security
---
