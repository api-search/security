---
api_specs:
- filename: netbox-openapi.yml
  format: yaml
  label: NetBox REST API
  slug: netbox-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox/refs/heads/main/openapi/netbox-openapi.yml
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
- Data Center
- DCIM
- Infrastructure as Code
- IPAM
- Network Automation
- Network Management
- Open Source
- Source of Truth
---
