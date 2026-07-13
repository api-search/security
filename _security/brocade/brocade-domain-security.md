---
api_specs:
- filename: brocade-openapi.yml
  format: yaml
  label: Brocade Fabric OS REST API
  slug: brocade-fabric-os-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brocade/refs/heads/main/openapi/brocade-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: broadcom.com
  spf: true
hosts:
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: techdocs.broadcom.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 20 23:59:59 2027 GMT
  host: www.broadcom.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 20 23:59:59 2027 GMT
  host: docs.broadcom.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brocade Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brocade, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Brocade
provider_slug: brocade
slug: brocade-domain-security
source_filename: brocade-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: techdocs.broadcom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.broadcom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.broadcom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: broadcom.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brocade/refs/heads/main/security/brocade-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Data Center
- Directors
- Fibre Channel
- Network Automation
- Networking
- SAN
- Storage Area Networks
- Switches
- Fortune 1000
---
