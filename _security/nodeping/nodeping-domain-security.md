---
api_specs:
- filename: nodeping-accounts-api-openapi.yml
  format: yaml
  label: NodePing Accounts API
  slug: nodeping-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nodeping/refs/heads/main/openapi/nodeping-accounts-api-openapi.yml
- filename: nodeping-checks-api-openapi.yml
  format: yaml
  label: NodePing Checks API
  slug: nodeping-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nodeping/refs/heads/main/openapi/nodeping-checks-api-openapi.yml
- filename: nodeping-contactgroups-api-openapi.yml
  format: yaml
  label: NodePing Contactgroups API
  slug: nodeping-contactgroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nodeping/refs/heads/main/openapi/nodeping-contactgroups-api-openapi.yml
- filename: nodeping-contacts-api-openapi.yml
  format: yaml
  label: NodePing Contacts API
  slug: nodeping-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nodeping/refs/heads/main/openapi/nodeping-contacts-api-openapi.yml
- filename: nodeping-info-api-openapi.yml
  format: yaml
  label: NodePing Info API
  slug: nodeping-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nodeping/refs/heads/main/openapi/nodeping-info-api-openapi.yml
- filename: nodeping-notifications-api-openapi.yml
  format: yaml
  label: NodePing Notifications API
  slug: nodeping-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nodeping/refs/heads/main/openapi/nodeping-notifications-api-openapi.yml
- filename: nodeping-results-api-openapi.yml
  format: yaml
  label: NodePing Results API
  slug: nodeping-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nodeping/refs/heads/main/openapi/nodeping-results-api-openapi.yml
- filename: nodeping-schedules-api-openapi.yml
  format: yaml
  label: NodePing Schedules API
  slug: nodeping-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nodeping/refs/heads/main/openapi/nodeping-schedules-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild "sectigo.com"
  - 0 iodef "mailto:support@nodeping.com"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nodeping.com
  spf: true
hosts:
- cert_expires: Dec 16 23:59:59 2026 GMT
  host: nodeping.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 16 23:59:59 2026 GMT
  host: api.nodeping.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nodeping Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NodePing, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: NodePing
provider_slug: nodeping
slug: nodeping-domain-security
source_filename: nodeping-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nodeping.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 23:59:59 2026 GMT\n  hsts: false\n- host: api.nodeping.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: nodeping.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 iodef \"mailto:support@nodeping.com\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nodeping/refs/heads/main/security/nodeping-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Monitoring
- Uptime
- Notification
- Software-as-a-Service
---
