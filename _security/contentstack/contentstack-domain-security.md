---
api_specs:
- filename: contentstack-content-delivery-api-openapi.yml
  format: yaml
  label: Contentstack Content Delivery API
  slug: content-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contentstack/refs/heads/main/openapi/contentstack-content-delivery-api-openapi.yml
- filename: contentstack-content-management-api-openapi.yml
  format: yaml
  label: Contentstack Content Management API
  slug: content-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contentstack/refs/heads/main/openapi/contentstack-content-management-api-openapi.yml
- filename: contentstack-personalize-management-api-openapi.yml
  format: yaml
  label: Contentstack Personalize Management API
  slug: personalize-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contentstack/refs/heads/main/openapi/contentstack-personalize-management-api-openapi.yml
- filename: contentstack-personalize-edge-api-openapi.yml
  format: yaml
  label: Contentstack Personalize Edge API
  slug: personalize-edge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contentstack/refs/heads/main/openapi/contentstack-personalize-edge-api-openapi.yml
- filename: contentstack-automate-management-api-openapi.yml
  format: yaml
  label: Contentstack Automate Management API
  slug: automate-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contentstack/refs/heads/main/openapi/contentstack-automate-management-api-openapi.yml
- filename: contentstack-analytics-api-openapi.yml
  format: yaml
  label: Contentstack Analytics API
  slug: analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contentstack/refs/heads/main/openapi/contentstack-analytics-api-openapi.yml
- filename: contentstack-scim-api-openapi.yml
  format: yaml
  label: Contentstack SCIM API
  slug: scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contentstack/refs/heads/main/openapi/contentstack-scim-api-openapi.yml
- filename: contentstack-brand-kit-management-api-openapi.yml
  format: yaml
  label: Contentstack Brand Kit Management API
  slug: brand-kit-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contentstack/refs/heads/main/openapi/contentstack-brand-kit-management-api-openapi.yml
- filename: contentstack-knowledge-vault-api-openapi.yml
  format: yaml
  label: Contentstack Knowledge Vault API
  slug: knowledge-vault-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contentstack/refs/heads/main/openapi/contentstack-knowledge-vault-api-openapi.yml
- filename: contentstack-generative-ai-api-openapi.yml
  format: yaml
  label: Contentstack Generative AI API
  slug: generative-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contentstack/refs/heads/main/openapi/contentstack-generative-ai-api-openapi.yml
- filename: contentstack-launch-api-openapi.yml
  format: yaml
  label: Contentstack Launch API
  slug: launch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contentstack/refs/heads/main/openapi/contentstack-launch-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: contentstack.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: contentstack.io
  spf: false
hosts:
- cert_expires: Sep 26 19:44:15 2026 GMT
  host: www.contentstack.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: cdn.contentstack.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: api.contentstack.io
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Contentstack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for contentstack, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: contentstack
provider_slug: contentstack
slug: contentstack-domain-security
source_filename: contentstack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.contentstack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 19:44:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: cdn.contentstack.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: null\n- host: api.contentstack.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: contentstack.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: contentstack.io\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild\
  \ \"globalsign.com\"\n  - 0 issuewild \"sectigo.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contentstack/refs/heads/main/security/contentstack-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags: []
---
