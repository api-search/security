---
api_specs:
- filename: packet-host-metal-openapi-original.yml
  format: yaml
  label: Metal API
  slug: metal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/packet-host/refs/heads/main/openapi/packet-host-metal-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: equinix.com
  spf: true
hosts:
- cert_expires: Feb  5 23:59:59 2027 GMT
  host: api.equinix.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Packet Host Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Packet Host, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Packet Host
provider_slug: packet-host
slug: packet-host-domain-security
source_filename: packet-host-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.equinix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: equinix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/packet-host/refs/heads/main/security/packet-host-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Bare Metal
- Cloud Infrastructure
- Infrastructure as a Service
- Servers
- Compute
- Provisioning
- Equinix Metal
- Retired
---
