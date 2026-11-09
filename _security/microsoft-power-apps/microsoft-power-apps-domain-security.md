---
api_specs:
- filename: microsoft-power-apps-accounts-api-openapi.yml
  format: yaml
  label: Microsoft Power Apps Accounts API
  slug: microsoft-power-apps-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-power-apps/openapi/microsoft-power-apps-accounts-api-openapi.yml
- filename: microsoft-power-apps-contacts-api-openapi.yml
  format: yaml
  label: Microsoft Power Apps Contacts API
  slug: microsoft-power-apps-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-power-apps/openapi/microsoft-power-apps-contacts-api-openapi.yml
- filename: microsoft-power-apps-entities-api-openapi.yml
  format: yaml
  label: Microsoft Power Apps Entities API
  slug: microsoft-power-apps-entities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-power-apps/openapi/microsoft-power-apps-entities-api-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: powerapps.com
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
hosts:
- cert_expires: Jan 21 18:34:57 2027 GMT
  host: make.powerapps.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 17 19:55:21 2027 GMT
  host: www.microsoft.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  7 23:37:09 2027 GMT
  host: docs.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Microsoft Power Apps Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Power Apps, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Microsoft Power Apps
provider_slug: microsoft-power-apps
slug: microsoft-power-apps-domain-security
source_filename: microsoft-power-apps-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: make.powerapps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 18:34:57 2027 GMT\n  hsts: null\n- host: www.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 19:55:21 2027 GMT\n  hsts: false\n- host: docs.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  7 23:37:09 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: powerapps.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/microsoft-power-apps/security/microsoft-power-apps-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Business Applications
- Cloud
- Enterprise
- Low-Code
- Microsoft
- No-Code
- Power Platform
- Software-as-a-Service
---
