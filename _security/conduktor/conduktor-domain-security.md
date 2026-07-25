---
api_specs:
- filename: conduktor-certificates-api-openapi.yml
  format: yaml
  label: Conduktor Certificates API
  slug: conduktor-certificates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conduktor/refs/heads/main/openapi/conduktor-certificates-api-openapi.yml
- filename: conduktor-clusters-api-openapi.yml
  format: yaml
  label: Conduktor Clusters API
  slug: conduktor-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conduktor/refs/heads/main/openapi/conduktor-clusters-api-openapi.yml
- filename: conduktor-groups-api-openapi.yml
  format: yaml
  label: Conduktor Groups API
  slug: conduktor-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conduktor/refs/heads/main/openapi/conduktor-groups-api-openapi.yml
- filename: conduktor-interceptors-api-openapi.yml
  format: yaml
  label: Conduktor Interceptors API
  slug: conduktor-interceptors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conduktor/refs/heads/main/openapi/conduktor-interceptors-api-openapi.yml
- filename: conduktor-self-service-api-openapi.yml
  format: yaml
  label: Conduktor Self-Service API
  slug: conduktor-self-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conduktor/refs/heads/main/openapi/conduktor-self-service-api-openapi.yml
- filename: conduktor-users-api-openapi.yml
  format: yaml
  label: Conduktor Users API
  slug: conduktor-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conduktor/refs/heads/main/openapi/conduktor-users-api-openapi.yml
- filename: conduktor-virtual-clusters-api-openapi.yml
  format: yaml
  label: Conduktor Virtual Clusters API
  slug: conduktor-virtual-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conduktor/refs/heads/main/openapi/conduktor-virtual-clusters-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: conduktor.io
  spf: true
hosts:
- cert_expires: Aug 26 21:30:36 2026 GMT
  host: www.conduktor.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 13:34:51 2026 GMT
  host: docs.conduktor.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Conduktor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Conduktor, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Conduktor
provider_slug: conduktor
slug: conduktor-domain-security
source_filename: conduktor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.conduktor.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 21:30:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.conduktor.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 13:34:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: conduktor.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conduktor/refs/heads/main/security/conduktor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Apache Kafka
- Streaming
- Data Governance
- Kafka Management
- Gateway
---
