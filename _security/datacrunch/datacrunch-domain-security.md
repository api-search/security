---
api_specs:
- filename: datacrunch-openapi.yml
  format: yaml
  label: DataCrunch Instances API
  slug: instances
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacrunch/refs/heads/main/openapi/datacrunch-openapi.yml
- filename: datacrunch-openapi.yml
  format: yaml
  label: DataCrunch Instance Types & Availability API
  slug: instance-types
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacrunch/refs/heads/main/openapi/datacrunch-openapi.yml
- filename: datacrunch-openapi.yml
  format: yaml
  label: DataCrunch Images & Startup Scripts API
  slug: images
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacrunch/refs/heads/main/openapi/datacrunch-openapi.yml
- filename: datacrunch-openapi.yml
  format: yaml
  label: DataCrunch SSH Keys API
  slug: ssh-keys
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacrunch/refs/heads/main/openapi/datacrunch-openapi.yml
- filename: datacrunch-openapi.yml
  format: yaml
  label: DataCrunch Volumes API
  slug: volumes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacrunch/refs/heads/main/openapi/datacrunch-openapi.yml
- filename: datacrunch-openapi.yml
  format: yaml
  label: DataCrunch Serverless Inference & Containers API
  slug: serverless-inference
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacrunch/refs/heads/main/openapi/datacrunch-openapi.yml
- filename: datacrunch-openapi.yml
  format: yaml
  label: DataCrunch Balance API
  slug: balance
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacrunch/refs/heads/main/openapi/datacrunch-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: datacrunch.io
  spf: true
hosts:
- cert_expires: Aug 21 14:48:05 2026 GMT
  host: datacrunch.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 16:14:07 2026 GMT
  host: api.datacrunch.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 10:13:57 2026 GMT
  host: docs.datacrunch.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Datacrunch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DataCrunch, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DataCrunch
provider_slug: datacrunch
slug: datacrunch-domain-security
source_filename: datacrunch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datacrunch.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 14:48:05 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.datacrunch.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 16:14:07 2026 GMT\n  hsts: null\n- host: docs.datacrunch.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 10:13:57 2026 GMT\n  hsts: false\ndomains:\n- domain: datacrunch.io\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datacrunch/refs/heads/main/security/datacrunch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- GPU Cloud
- Infrastructure
- Compute
- Inference
- Serverless
- Europe
---
