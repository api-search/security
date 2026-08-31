---
api_specs:
- filename: infinidat-components-api-openapi.yml
  format: yaml
  label: Infinidat Components API
  slug: infinidat-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infinidat/refs/heads/main/openapi/infinidat-components-api-openapi.yml
- filename: infinidat-config-api-openapi.yml
  format: yaml
  label: Infinidat Config API
  slug: infinidat-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infinidat/refs/heads/main/openapi/infinidat-config-api-openapi.yml
- filename: infinidat-filesystems-api-openapi.yml
  format: yaml
  label: Infinidat Filesystems API
  slug: infinidat-filesystems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infinidat/refs/heads/main/openapi/infinidat-filesystems-api-openapi.yml
- filename: infinidat-hosts-api-openapi.yml
  format: yaml
  label: Infinidat Hosts API
  slug: infinidat-hosts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infinidat/refs/heads/main/openapi/infinidat-hosts-api-openapi.yml
- filename: infinidat-metadata-api-openapi.yml
  format: yaml
  label: Infinidat Metadata API
  slug: infinidat-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infinidat/refs/heads/main/openapi/infinidat-metadata-api-openapi.yml
- filename: infinidat-pools-api-openapi.yml
  format: yaml
  label: Infinidat Pools API
  slug: infinidat-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infinidat/refs/heads/main/openapi/infinidat-pools-api-openapi.yml
- filename: infinidat-system-api-openapi.yml
  format: yaml
  label: Infinidat System API
  slug: infinidat-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infinidat/refs/heads/main/openapi/infinidat-system-api-openapi.yml
- filename: infinidat-users-api-openapi.yml
  format: yaml
  label: Infinidat Users API
  slug: infinidat-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infinidat/refs/heads/main/openapi/infinidat-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: infinidat.com
  spf: true
hosts:
- cert_expires: Sep  8 08:22:52 2026 GMT
  host: www.infinidat.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 23:46:13 2026 GMT
  host: support.infinidat.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Infinidat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Infinidat, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Infinidat
provider_slug: infinidat
slug: infinidat-domain-security
source_filename: infinidat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.infinidat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 08:22:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: support.infinidat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:46:13 2026 GMT\n  hsts: null\ndomains:\n- domain: infinidat.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infinidat/refs/heads/main/security/infinidat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Storage
- Enterprise Storage
- Data Infrastructure
- Data Protection
- Cyber Resilience
- Backup and Recovery
- Kubernetes
- Infrastructure
- On-Premises
---
