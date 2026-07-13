---
api_specs:
- filename: hawksoft-openapi.yml
  format: yaml
  label: HawkSoft Agencies and Offices API
  slug: hawksoft-agencies-offices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hawksoft/refs/heads/main/openapi/hawksoft-openapi.yml
- filename: hawksoft-openapi.yml
  format: yaml
  label: HawkSoft Clients API
  slug: hawksoft-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hawksoft/refs/heads/main/openapi/hawksoft-openapi.yml
- filename: hawksoft-openapi.yml
  format: yaml
  label: HawkSoft Log Entries API
  slug: hawksoft-log-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hawksoft/refs/heads/main/openapi/hawksoft-openapi.yml
- filename: hawksoft-openapi.yml
  format: yaml
  label: HawkSoft Attachments and Receipts API
  slug: hawksoft-attachments-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hawksoft/refs/heads/main/openapi/hawksoft-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hawksoft.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: hawksoft.app
  spf: true
hosts:
- cert_expires: Aug 21 23:59:59 2026 GMT
  host: www.hawksoft.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: partner.hawksoft.app
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: integration.hawksoft.app
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hawksoft Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HawkSoft, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: HawkSoft
provider_slug: hawksoft
slug: hawksoft-domain-security
source_filename: hawksoft-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hawksoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 23:59:59 2026 GMT\n  hsts: false\n- host: partner.hawksoft.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: false\n- host: integration.hawksoft.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: hawksoft.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: hawksoft.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hawksoft/refs/heads/main/security/hawksoft-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Insurance
- Agency Management System
- AMS
- InsurTech
- Property and Casualty
- Partner API
- Gated API
---
