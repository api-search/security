---
api_specs:
- filename: netbox-labs-authentication-check-api-openapi.yml
  format: yaml
  label: NetBox Labs authentication-check API
  slug: netbox-labs-authentication-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox-labs/refs/heads/main/openapi/netbox-labs-authentication-check-api-openapi.yml
- filename: netbox-labs-circuits-api-openapi.yml
  format: yaml
  label: NetBox Labs circuits API
  slug: netbox-labs-circuits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox-labs/refs/heads/main/openapi/netbox-labs-circuits-api-openapi.yml
- filename: netbox-labs-core-api-openapi.yml
  format: yaml
  label: NetBox Labs core API
  slug: netbox-labs-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox-labs/refs/heads/main/openapi/netbox-labs-core-api-openapi.yml
- filename: netbox-labs-dcim-api-openapi.yml
  format: yaml
  label: NetBox Labs dcim API
  slug: netbox-labs-dcim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox-labs/refs/heads/main/openapi/netbox-labs-dcim-api-openapi.yml
- filename: netbox-labs-extras-api-openapi.yml
  format: yaml
  label: NetBox Labs extras API
  slug: netbox-labs-extras-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox-labs/refs/heads/main/openapi/netbox-labs-extras-api-openapi.yml
- filename: netbox-labs-ipam-api-openapi.yml
  format: yaml
  label: NetBox Labs ipam API
  slug: netbox-labs-ipam-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox-labs/refs/heads/main/openapi/netbox-labs-ipam-api-openapi.yml
- filename: netbox-labs-schema-api-openapi.yml
  format: yaml
  label: NetBox Labs schema API
  slug: netbox-labs-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox-labs/refs/heads/main/openapi/netbox-labs-schema-api-openapi.yml
- filename: netbox-labs-status-api-openapi.yml
  format: yaml
  label: NetBox Labs status API
  slug: netbox-labs-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox-labs/refs/heads/main/openapi/netbox-labs-status-api-openapi.yml
- filename: netbox-labs-tenancy-api-openapi.yml
  format: yaml
  label: NetBox Labs tenancy API
  slug: netbox-labs-tenancy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox-labs/refs/heads/main/openapi/netbox-labs-tenancy-api-openapi.yml
- filename: netbox-labs-users-api-openapi.yml
  format: yaml
  label: NetBox Labs users API
  slug: netbox-labs-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox-labs/refs/heads/main/openapi/netbox-labs-users-api-openapi.yml
- filename: netbox-labs-virtualization-api-openapi.yml
  format: yaml
  label: NetBox Labs virtualization API
  slug: netbox-labs-virtualization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox-labs/refs/heads/main/openapi/netbox-labs-virtualization-api-openapi.yml
- filename: netbox-labs-vpn-api-openapi.yml
  format: yaml
  label: NetBox Labs vpn API
  slug: netbox-labs-vpn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox-labs/refs/heads/main/openapi/netbox-labs-vpn-api-openapi.yml
- filename: netbox-labs-wireless-api-openapi.yml
  format: yaml
  label: NetBox Labs wireless API
  slug: netbox-labs-wireless-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox-labs/refs/heads/main/openapi/netbox-labs-wireless-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: netboxlabs.com
  spf: true
hosts:
- cert_expires: Aug 21 23:00:20 2026 GMT
  host: netboxlabs.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Netbox Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NetBox Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: NetBox Labs
provider_slug: netbox-labs
slug: netbox-labs-domain-security
source_filename: netbox-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: netboxlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 23:00:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: netboxlabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/netbox-labs/refs/heads/main/security/netbox-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Networking
- DCIM
- IPAM
- Infrastructure
- Source of Truth
- Network Automation
- OpenAPI
- MCP
---
