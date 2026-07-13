---
api_specs:
- filename: ariba-sourcing-external-approval-api.yaml
  format: yaml
  label: Ariba Sourcing - External Approval API
  slug: ariba-sourcing-external-approval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ariba-sourcing/refs/heads/main/openapi/ariba-sourcing-external-approval-api.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ariba.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sap.com
  spf: true
hosts:
- cert_expires: Mar 22 23:59:59 2027 GMT
  host: developer.ariba.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: help.sap.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 22 23:59:59 2027 GMT
  host: openapi.ariba.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ariba Sourcing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ariba Sourcing, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ariba Sourcing
provider_slug: ariba-sourcing
slug: ariba-sourcing-domain-security
source_filename: ariba-sourcing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.ariba.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: help.sap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: openapi.ariba.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 22 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: ariba.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: sap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ariba-sourcing/refs/heads/main/security/ariba-sourcing-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Approvals
- Auctions
- B2B
- Contracts
- Procurement
- RFx
- SAP
- Sourcing
- Supplier Management
- Supply Chain
---
