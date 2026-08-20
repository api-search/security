---
api_specs:
- filename: spredfast-conversations-api-openapi.yml
  format: yaml
  label: Spredfast Conversations API (v2)
  slug: spredfast-conversations-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spredfast/refs/heads/main/openapi/spredfast-conversations-api-openapi.yml
- filename: spredfast-conversations-api-v1-openapi.yml
  format: yaml
  label: Spredfast Conversations API (v1)
  slug: spredfast-conversations-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spredfast/refs/heads/main/openapi/spredfast-conversations-api-v1-openapi.yml
- filename: spredfast-analytics-api-openapi.yml
  format: yaml
  label: Spredfast Analytics Reporting API
  slug: spredfast-analytics-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spredfast/refs/heads/main/openapi/spredfast-analytics-api-openapi.yml
- filename: spredfast-notification-api-openapi.yml
  format: yaml
  label: Spredfast Notifications (Events) API
  slug: spredfast-notifications-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spredfast/refs/heads/main/openapi/spredfast-notification-api-openapi.yml
- filename: spredfast-experiences-stream-api-openapi.yml
  format: yaml
  label: Spredfast Experiences Stream API
  slug: spredfast-experiences-stream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spredfast/refs/heads/main/openapi/spredfast-experiences-stream-api-openapi.yml
- filename: spredfast-crm-api-openapi.yml
  format: yaml
  label: Spredfast CRM Registration API
  slug: spredfast-crm-registration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spredfast/refs/heads/main/openapi/spredfast-crm-api-openapi.yml
- filename: spredfast-custom-crm-callback-api-openapi.yml
  format: yaml
  label: Spredfast Custom CRM Callback Contract
  slug: spredfast-custom-crm-callback-contract
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spredfast/refs/heads/main/openapi/spredfast-custom-crm-callback-api-openapi.yml
- filename: spredfast-labelsets-api-openapi.yml
  format: yaml
  label: Spredfast Label Sets API
  slug: spredfast-label-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spredfast/refs/heads/main/openapi/spredfast-labelsets-api-openapi.yml
- filename: spredfast-introspection-api-openapi.yml
  format: yaml
  label: Spredfast Introspection API
  slug: spredfast-introspection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spredfast/refs/heads/main/openapi/spredfast-introspection-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "globalsign.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: khoros.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: spredfast.com
  spf: true
hosts:
- cert_expires: Oct  3 20:18:28 2026 GMT
  host: developer.khoros.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: api.spredfast.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 13 23:59:59 2027 GMT
  host: api.massrelevance.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spredfast Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spredfast, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Spredfast
provider_slug: spredfast
slug: spredfast-domain-security
source_filename: spredfast-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.khoros.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 20:18:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.spredfast.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: null\n- host: api.massrelevance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: khoros.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: spredfast.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spredfast/refs/heads/main/security/spredfast-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Social-Media
- Social Media Management
- Marketing
- Social Marketing
- Publishing
- Analytics
- Engagement
- Content Management
- Webhook
- Event
- Enterprise
---
