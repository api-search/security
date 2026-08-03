---
api_specs:
- filename: nerdio-distributor-api-openapi.json
  format: json
  label: Nerdio Manager Distributor API
  slug: nerdio-manager-distributor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nerdio/refs/heads/main/openapi/nerdio-distributor-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: getnerdio.com
  spf: true
- caa:
  - 0 issue "godaddy.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nerdio.net
  spf: true
hosts:
- cert_expires: Oct 18 23:20:19 2026 GMT
  host: getnerdio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 18:26:51 2026 GMT
  host: nmmhelp.getnerdio.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: nmm-distributor-api.nerdio.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nerdio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nerdio, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nerdio
provider_slug: nerdio
slug: nerdio-domain-security
source_filename: nerdio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getnerdio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:20:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: nmmhelp.getnerdio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 18:26:51 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n- host: nmm-distributor-api.nerdio.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: getnerdio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: nerdio.net\n  dnssec: false\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nerdio/refs/heads/main/security/nerdio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Azure Virtual Desktop
- Windows 365
- Virtual Desktop Infrastructure
- Cloud Desktop Management
- Microsoft Intune
- Managed Service Providers
- Cloud Cost Optimization
- Endpoint Management
- IT Automation
---
