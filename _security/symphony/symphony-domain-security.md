---
api_specs:
- filename: symphony-all-api-openapi.yml
  format: yaml
  label: Symphony All API
  slug: symphony-all-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/symphony-all-api-openapi.yml
- filename: symphony-app-api-openapi.yml
  format: yaml
  label: Symphony App API
  slug: symphony-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/symphony-app-api-openapi.yml
- filename: symphony-audittrail-api-openapi.yml
  format: yaml
  label: Symphony Audittrail API
  slug: symphony-audittrail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/symphony-audittrail-api-openapi.yml
- filename: symphony-authenticate-api-openapi.yml
  format: yaml
  label: Symphony Authenticate API
  slug: symphony-authenticate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/symphony-authenticate-api-openapi.yml
- filename: symphony-channelco-api-openapi.yml
  format: yaml
  label: Symphony Channelco API
  slug: symphony-channelco-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/symphony-channelco-api-openapi.yml
- filename: symphony-datafeeds-api-openapi.yml
  format: yaml
  label: Symphony Datafeeds API
  slug: symphony-datafeeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/symphony-datafeeds-api-openapi.yml
- filename: symphony-dlp-api-openapi.yml
  format: yaml
  label: Symphony Dlp API
  slug: symphony-dlp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/symphony-dlp-api-openapi.yml
- filename: symphony-events-api-openapi.yml
  format: yaml
  label: Symphony Events API
  slug: symphony-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/symphony-events-api-openapi.yml
- filename: symphony-groups-api-openapi.yml
  format: yaml
  label: Symphony Groups API
  slug: symphony-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/symphony-groups-api-openapi.yml
- filename: symphony-health-api-openapi.yml
  format: yaml
  label: Symphony Health API
  slug: symphony-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/symphony-health-api-openapi.yml
- filename: symphony-idm-api-openapi.yml
  format: yaml
  label: Symphony Idm API
  slug: symphony-idm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/symphony-idm-api-openapi.yml
- filename: symphony-info-api-openapi.yml
  format: yaml
  label: Symphony Info API
  slug: symphony-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/symphony-info-api-openapi.yml
- filename: symphony-logout-api-openapi.yml
  format: yaml
  label: Symphony Logout API
  slug: symphony-logout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/symphony-logout-api-openapi.yml
- filename: symphony-message-api-openapi.yml
  format: yaml
  label: Symphony Message API
  slug: symphony-message-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/symphony-message-api-openapi.yml
- filename: symphony-onboarding-api-openapi.yml
  format: yaml
  label: Symphony Onboarding API
  slug: symphony-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/symphony-onboarding-api-openapi.yml
- filename: symphony-pubkey-api-openapi.yml
  format: yaml
  label: Symphony Pubkey API
  slug: symphony-pubkey-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/symphony-pubkey-api-openapi.yml
- filename: symphony-signals-api-openapi.yml
  format: yaml
  label: Symphony Signals API
  slug: symphony-signals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/symphony-signals-api-openapi.yml
- filename: symphony-stream-api-openapi.yml
  format: yaml
  label: Symphony Stream API
  slug: symphony-stream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/symphony-stream-api-openapi.yml
- filename: symphony-types-api-openapi.yml
  format: yaml
  label: Symphony Types API
  slug: symphony-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/symphony-types-api-openapi.yml
- filename: symphony-util-api-openapi.yml
  format: yaml
  label: Symphony Util API
  slug: symphony-util-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/symphony-util-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: symphony.com
  spf: true
hosts:
- cert_expires: Sep 30 03:48:59 2026 GMT
  host: symphony.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 30 03:48:59 2026 GMT
  host: developers.symphony.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.2
- host: acme.symphony.com
  https: false
kind: domain-security
layout: security
method: probed
name: Symphony Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Symphony, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Symphony
provider_slug: symphony
slug: symphony-domain-security
source_filename: symphony-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: symphony.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 30 03:48:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.symphony.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 30 03:48:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\n- host: acme.symphony.com\n  https: false\ndomains:\n- domain: symphony.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/security/symphony-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Collaboration
- Communications
- Financial-Services
- Messaging
- Secure Communication
---
