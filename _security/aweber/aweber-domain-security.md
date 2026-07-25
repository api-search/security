---
api_specs:
- filename: aweber-accounts-api-openapi.yml
  format: yaml
  label: AWeber Accounts API
  slug: aweber-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-accounts-api-openapi.yml
- filename: aweber-broadcasts-api-openapi.yml
  format: yaml
  label: AWeber Broadcasts API
  slug: aweber-broadcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-broadcasts-api-openapi.yml
- filename: aweber-campaigns-api-openapi.yml
  format: yaml
  label: AWeber Campaigns API
  slug: aweber-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-campaigns-api-openapi.yml
- filename: aweber-custom-fields-api-openapi.yml
  format: yaml
  label: AWeber Custom Fields API
  slug: aweber-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-custom-fields-api-openapi.yml
- filename: aweber-landing-pages-api-openapi.yml
  format: yaml
  label: AWeber Landing Pages API
  slug: aweber-landing-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-landing-pages-api-openapi.yml
- filename: aweber-lists-api-openapi.yml
  format: yaml
  label: AWeber Lists API
  slug: aweber-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-lists-api-openapi.yml
- filename: aweber-segments-api-openapi.yml
  format: yaml
  label: AWeber Segments API
  slug: aweber-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-segments-api-openapi.yml
- filename: aweber-subscribers-api-openapi.yml
  format: yaml
  label: AWeber Subscribers API
  slug: aweber-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-subscribers-api-openapi.yml
- filename: aweber-web-forms-api-openapi.yml
  format: yaml
  label: AWeber Web Forms API
  slug: aweber-web-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-web-forms-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aweber.com
  spf: true
hosts:
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: www.aweber.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: developer.aweber.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: api.aweber.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Aweber Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AWeber, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AWeber
provider_slug: aweber
slug: aweber-domain-security
source_filename: aweber-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aweber.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: false\n- host: developer.aweber.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: false\n- host: api.aweber.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: aweber.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/security/aweber-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Email Marketing
- Marketing Automation
- Email
- Newsletters
- Subscribers
- Campaigns
- Landing Pages
---
