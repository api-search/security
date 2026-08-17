---
api_specs:
- filename: emotive-open-api-openapi.yml
  format: yaml
  label: Emotive Open API
  slug: emotive-open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emotive/refs/heads/main/openapi/emotive-open-api-openapi.yml
- filename: emotive-subscriber-engine-openapi.yml
  format: yaml
  label: Emotive Lists API (Subscriber Engine)
  slug: emotive-lists-api-subscriber-engine
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emotive/refs/heads/main/openapi/emotive-subscriber-engine-openapi.yml
- filename: emotive-sensus-webhook-openapi.yml
  format: yaml
  label: Emotive Sensus Webhooks API
  slug: emotive-sensus-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emotive/refs/heads/main/openapi/emotive-sensus-webhook-openapi.yml
- filename: emotive-helpdesk-openapi.yml
  format: yaml
  label: Emotive Helpdesk API
  slug: emotive-helpdesk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emotive/refs/heads/main/openapi/emotive-helpdesk-openapi.yml
- filename: emotive-auth-openapi.yml
  format: yaml
  label: Emotive Auth Server API
  slug: emotive-auth-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emotive/refs/heads/main/openapi/emotive-auth-openapi.yml
- filename: emotive-segments-openapi.yml
  format: yaml
  label: Emotive Segments API
  slug: emotive-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emotive/refs/heads/main/openapi/emotive-segments-openapi.yml
- filename: emotive-experiences-openapi.yml
  format: yaml
  label: Emotive Experiences API
  slug: emotive-experiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emotive/refs/heads/main/openapi/emotive-experiences-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: emotive.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: emotiveapp.co
  spf: false
hosts:
- cert_expires: Jan 30 23:59:59 2027 GMT
  host: www.emotive.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 21 23:59:59 2027 GMT
  host: api-gw.emotiveapp.co
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: api.emotiveapp.co
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Emotive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Emotive, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Emotive
provider_slug: emotive
slug: emotive-domain-security
source_filename: emotive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.emotive.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  hsts: false\n- host: api-gw.emotiveapp.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 21 23:59:59 2027 GMT\n  hsts: null\n- host: api.emotiveapp.co\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: emotive.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: emotiveapp.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emotive/refs/heads/main/security/emotive-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Marketing
- SMS
- Messaging
- eCommerce
- Marketing Automation
- Text Message Marketing
- Conversational Commerce
- Webhooks
- Customer Data
- Segmentation
- Attribution
---
