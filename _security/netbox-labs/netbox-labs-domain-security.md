---
api_specs:
- filename: netbox-labs-openapi-original.json
  format: json
  label: NetBox REST API
  slug: netbox-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox-labs/refs/heads/main/openapi/netbox-labs-openapi-original.json
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
