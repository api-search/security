---
api_specs:
- filename: openstack-domains-api-openapi.yml
  format: yaml
  label: OpenStack Domains API
  slug: openstack-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-domains-api-openapi.yml
- filename: openstack-endpoints-api-openapi.yml
  format: yaml
  label: OpenStack Endpoints API
  slug: openstack-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-endpoints-api-openapi.yml
- filename: openstack-flavors-api-openapi.yml
  format: yaml
  label: OpenStack Flavors API
  slug: openstack-flavors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-flavors-api-openapi.yml
- filename: openstack-groups-api-openapi.yml
  format: yaml
  label: OpenStack Groups API
  slug: openstack-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-groups-api-openapi.yml
- filename: openstack-images-api-openapi.yml
  format: yaml
  label: OpenStack Images API
  slug: openstack-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-images-api-openapi.yml
- filename: openstack-keypairs-api-openapi.yml
  format: yaml
  label: OpenStack Keypairs API
  slug: openstack-keypairs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-keypairs-api-openapi.yml
- filename: openstack-projects-api-openapi.yml
  format: yaml
  label: OpenStack Projects API
  slug: openstack-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-projects-api-openapi.yml
- filename: openstack-roles-api-openapi.yml
  format: yaml
  label: OpenStack Roles API
  slug: openstack-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-roles-api-openapi.yml
- filename: openstack-server-actions-api-openapi.yml
  format: yaml
  label: OpenStack Server Actions API
  slug: openstack-server-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-server-actions-api-openapi.yml
- filename: openstack-servers-api-openapi.yml
  format: yaml
  label: OpenStack Servers API
  slug: openstack-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-servers-api-openapi.yml
- filename: openstack-services-api-openapi.yml
  format: yaml
  label: OpenStack Services API
  slug: openstack-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-services-api-openapi.yml
- filename: openstack-tokens-api-openapi.yml
  format: yaml
  label: OpenStack Tokens API
  slug: openstack-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-tokens-api-openapi.yml
- filename: openstack-users-api-openapi.yml
  format: yaml
  label: OpenStack Users API
  slug: openstack-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-users-api-openapi.yml
- filename: openstack-versions-api-openapi.yml
  format: yaml
  label: OpenStack Versions API
  slug: openstack-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-versions-api-openapi.yml
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openstack.org
  spf: true
hosts:
- cert_expires: Sep 17 23:43:47 2026 GMT
  host: www.openstack.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 18:11:11 2026 GMT
  host: docs.openstack.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openstack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenStack, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OpenStack
provider_slug: openstack
slug: openstack-domain-security
source_filename: openstack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.openstack.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 23:43:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.openstack.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 18:11:11 2026 GMT\n  hsts: false\ndomains:\n- domain: openstack.org\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/security/openstack-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Platform
- Infrastructure as a Service
- Open Source
- Virtualization
- Linux Foundation
---
