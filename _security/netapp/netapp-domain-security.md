---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: NetApp Cloud Manager API
  slug: netapp-cloud-manager-api
  spec_type: OpenAPI
  url: https://docs.netapp.com/us-en/cloud-manager-automation/api/openapi.yaml
- filename: netapp-ontap-openapi.yml
  format: yaml
  label: NetApp ONTAP REST API
  slug: netapp-ontap-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netapp/refs/heads/main/openapi/netapp-ontap-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: netapp.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
hosts:
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: docs.netapp.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: cloudmanager.cloud.netapp.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:35:22 2026 GMT
  host: cloud.google.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Netapp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NetApp, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: NetApp
provider_slug: netapp
slug: netapp-domain-security
source_filename: netapp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.netapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: cloudmanager.cloud.netapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: null\n- host: cloud.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: netapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/netapp/refs/heads/main/security/netapp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud
- Data Management
- Hybrid Cloud
- Infrastructure
- Storage
- Fortune 500
---
