---
api_specs:
- filename: netbox-authentication-check-api-openapi.yml
  format: yaml
  label: NetBox authentication-check API
  slug: netbox-authentication-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox/refs/heads/main/openapi/netbox-authentication-check-api-openapi.yml
- filename: netbox-circuits-api-openapi.yml
  format: yaml
  label: NetBox circuits API
  slug: netbox-circuits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox/refs/heads/main/openapi/netbox-circuits-api-openapi.yml
- filename: netbox-core-api-openapi.yml
  format: yaml
  label: NetBox core API
  slug: netbox-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox/refs/heads/main/openapi/netbox-core-api-openapi.yml
- filename: netbox-dcim-api-openapi.yml
  format: yaml
  label: NetBox dcim API
  slug: netbox-dcim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox/refs/heads/main/openapi/netbox-dcim-api-openapi.yml
- filename: netbox-extras-api-openapi.yml
  format: yaml
  label: NetBox extras API
  slug: netbox-extras-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox/refs/heads/main/openapi/netbox-extras-api-openapi.yml
- filename: netbox-ipam-api-openapi.yml
  format: yaml
  label: NetBox ipam API
  slug: netbox-ipam-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox/refs/heads/main/openapi/netbox-ipam-api-openapi.yml
- filename: netbox-schema-api-openapi.yml
  format: yaml
  label: NetBox schema API
  slug: netbox-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox/refs/heads/main/openapi/netbox-schema-api-openapi.yml
- filename: netbox-status-api-openapi.yml
  format: yaml
  label: NetBox status API
  slug: netbox-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox/refs/heads/main/openapi/netbox-status-api-openapi.yml
- filename: netbox-tenancy-api-openapi.yml
  format: yaml
  label: NetBox tenancy API
  slug: netbox-tenancy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox/refs/heads/main/openapi/netbox-tenancy-api-openapi.yml
- filename: netbox-users-api-openapi.yml
  format: yaml
  label: NetBox users API
  slug: netbox-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox/refs/heads/main/openapi/netbox-users-api-openapi.yml
- filename: netbox-virtualization-api-openapi.yml
  format: yaml
  label: NetBox virtualization API
  slug: netbox-virtualization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox/refs/heads/main/openapi/netbox-virtualization-api-openapi.yml
- filename: netbox-vpn-api-openapi.yml
  format: yaml
  label: NetBox vpn API
  slug: netbox-vpn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox/refs/heads/main/openapi/netbox-vpn-api-openapi.yml
- filename: netbox-wireless-api-openapi.yml
  format: yaml
  label: NetBox wireless API
  slug: netbox-wireless-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox/refs/heads/main/openapi/netbox-wireless-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: netbox.dev
  spf: false
hosts:
- cert_expires: Aug 11 14:51:48 2026 GMT
  host: docs.netbox.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 23:39:56 2026 GMT
  host: demo.netbox.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Netbox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NetBox, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: NetBox
provider_slug: netbox
slug: netbox-domain-security
source_filename: netbox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.netbox.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 14:51:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: demo.netbox.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 23:39:56 2026 GMT\n  hsts: false\ndomains:\n- domain: netbox.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/netbox/refs/heads/main/security/netbox-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Data-Center
- DCIM
- Infrastructure as Code
- IPAM
- Network Automation
- Network Management
- Open-Source
- Source of Truth
---
