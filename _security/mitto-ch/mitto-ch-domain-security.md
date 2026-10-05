---
api_specs:
- filename: mitto-ch-apis-api-openapi.yml
  format: yaml
  label: Mitto APIs API
  slug: mitto-ch-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mitto-ch/refs/heads/main/openapi/mitto-ch-apis-api-openapi.yml
- filename: mitto-ch-autoreplyconfigs-api-openapi.yml
  format: yaml
  label: Mitto Auto Reply Configs API
  slug: mitto-ch-autoreplyconfigs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mitto-ch/refs/heads/main/openapi/mitto-ch-autoreplyconfigs-api-openapi.yml
- filename: mitto-ch-customers-api-openapi.yml
  format: yaml
  label: Mitto Customers API
  slug: mitto-ch-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mitto-ch/refs/heads/main/openapi/mitto-ch-customers-api-openapi.yml
- filename: mitto-ch-mitto-api-api-openapi.yml
  format: yaml
  label: Mitto Mitto API
  slug: mitto-ch-mitto-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mitto-ch/refs/heads/main/openapi/mitto-ch-mitto-api-api-openapi.yml
- filename: mitto-ch-statistic-api-openapi.yml
  format: yaml
  label: Mitto Statistic API
  slug: mitto-ch-statistic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mitto-ch/refs/heads/main/openapi/mitto-ch-statistic-api-openapi.yml
- filename: mitto-ch-webhooks-api-openapi.yml
  format: yaml
  label: Mitto Webhooks API
  slug: mitto-ch-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mitto-ch/refs/heads/main/openapi/mitto-ch-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mitto.ch
  spf: true
hosts:
- cert_expires: Apr 15 23:59:59 2027 GMT
  host: www.mitto.ch
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mitto Ch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mitto, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mitto
provider_slug: mitto-ch
slug: mitto-ch-domain-security
source_filename: mitto-ch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mitto.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 15 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mitto.ch\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mitto-ch/refs/heads/main/security/mitto-ch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Messaging
- Omnichannel
- Communications
- Enterprise
---
