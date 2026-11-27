---
api_specs:
- filename: mailfixture-com-domains-api-openapi.yml
  format: yaml
  label: mailfixture Domains API
  slug: mailfixture-com-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailfixture-com/openapi/mailfixture-com-domains-api-openapi.yml
- filename: mailfixture-com-hooks-api-openapi.yml
  format: yaml
  label: mailfixture Hooks API
  slug: mailfixture-com-hooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailfixture-com/openapi/mailfixture-com-hooks-api-openapi.yml
- filename: mailfixture-com-inboxes-api-openapi.yml
  format: yaml
  label: mailfixture Inboxes API
  slug: mailfixture-com-inboxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailfixture-com/openapi/mailfixture-com-inboxes-api-openapi.yml
- filename: mailfixture-com-keys-api-openapi.yml
  format: yaml
  label: mailfixture Keys API
  slug: mailfixture-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailfixture-com/openapi/mailfixture-com-keys-api-openapi.yml
- filename: mailfixture-com-messages-api-openapi.yml
  format: yaml
  label: mailfixture Messages API
  slug: mailfixture-com-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailfixture-com/openapi/mailfixture-com-messages-api-openapi.yml
- filename: mailfixture-com-phone-numbers-api-openapi.yml
  format: yaml
  label: mailfixture Phone Numbers API
  slug: mailfixture-com-phone-numbers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailfixture-com/openapi/mailfixture-com-phone-numbers-api-openapi.yml
- filename: mailfixture-com-sms-api-openapi.yml
  format: yaml
  label: mailfixture Sms API
  slug: mailfixture-com-sms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailfixture-com/openapi/mailfixture-com-sms-api-openapi.yml
- filename: mailfixture-com-webhooks-api-openapi.yml
  format: yaml
  label: mailfixture Webhooks API
  slug: mailfixture-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailfixture-com/openapi/mailfixture-com-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: mailfixture.com
  spf: true
hosts:
- cert_expires: Jan 30 18:49:54 2027 GMT
  host: mailfixture.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: mailfixture Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for mailfixture, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: mailfixture
provider_slug: mailfixture-com
slug: mailfixture-com-domain-security
source_filename: mailfixture-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mailfixture.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 18:49:54 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mailfixture.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/mailfixture-com/security/mailfixture-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Email
- Testing
- Developer Tools
- Automation
---
