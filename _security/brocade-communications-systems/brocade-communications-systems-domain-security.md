---
api_specs:
- filename: brocade-communications-systems-openapi.yml
  format: yaml
  label: Brocade Fabric OS REST API
  slug: fabric-os-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brocade-communications-systems/refs/heads/main/openapi/brocade-communications-systems-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: broadcom.com
  spf: true
hosts:
- cert_expires: Mar 20 23:59:59 2027 GMT
  host: www.broadcom.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: techdocs.broadcom.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brocade Communications Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brocade Communications Systems, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Brocade Communications Systems
provider_slug: brocade-communications-systems
slug: brocade-communications-systems-domain-security
source_filename: brocade-communications-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.broadcom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: techdocs.broadcom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: broadcom.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brocade-communications-systems/refs/heads/main/security/brocade-communications-systems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Data Networking
- Fibre Channel
- IP Networking
- Networking
- SAN
- Storage Networking
- Switches
- Fortune 1000
---
