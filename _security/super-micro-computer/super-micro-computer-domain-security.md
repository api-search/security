---
api_specs:
- filename: supermicro-redfish-openapi.yml
  format: yaml
  label: Supermicro Redfish API
  slug: redfish-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/super-micro-computer/refs/heads/main/openapi/supermicro-redfish-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: supermicro.com
  spf: true
hosts:
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: www.supermicro.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Super Micro Computer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Super Micro Computer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Super Micro Computer
provider_slug: super-micro-computer
slug: super-micro-computer-domain-security
source_filename: super-micro-computer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.supermicro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: supermicro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/super-micro-computer/refs/heads/main/security/super-micro-computer-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Servers
- Data Center
- Hardware
- Server Management
- Redfish
- BMC
- IPMI
- Fortune 500
- Infrastructure
- Cloud
---
