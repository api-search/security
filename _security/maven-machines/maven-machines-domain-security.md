---
api_specs:
- filename: maven-machines-users-openapi.json
  format: json
  label: Maven Integrations API
  slug: maven-machines-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maven-machines/refs/heads/main/openapi/maven-machines-users-openapi.json
- filename: maven-machines-aaa-cooper-middleware-openapi.json
  format: json
  label: Maven Customer Integration Middleware
  slug: maven-machines-customer-middleware
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maven-machines/refs/heads/main/openapi/maven-machines-aaa-cooper-middleware-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mavenmachines.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.io
  spf: true
hosts:
- cert_expires: Sep 10 23:59:59 2026 GMT
  host: mavenmachines.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  9 13:12:37 2026 GMT
  host: maven-machines.readme.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 23:59:59 2026 GMT
  host: integrations.mavenmachines.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Maven Machines Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Maven Machines, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Maven Machines
provider_slug: maven-machines
slug: maven-machines-domain-security
source_filename: maven-machines-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mavenmachines.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: maven-machines.readme.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:12:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: integrations.mavenmachines.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: mavenmachines.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: readme.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maven-machines/refs/heads/main/security/maven-machines-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Transportation
- Logistics
- Trucking
- Fleet Management
- Telematics
- ELD
- Route Optimization
- Dispatch
- Supply Chain
- Freight
---
