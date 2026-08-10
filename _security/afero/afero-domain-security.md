---
api_specs:
- filename: afero-authentication-api-openapi.yml
  format: yaml
  label: Afero Cloud Authentication API
  slug: authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afero/refs/heads/main/openapi/afero-authentication-api-openapi.yml
- filename: afero-users-api-openapi.yml
  format: yaml
  label: Afero Cloud Users API
  slug: users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afero/refs/heads/main/openapi/afero-users-api-openapi.yml
- filename: afero-devices-api-openapi.yml
  format: yaml
  label: Afero Cloud Devices API
  slug: devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afero/refs/heads/main/openapi/afero-devices-api-openapi.yml
- filename: afero-ota-api-openapi.yml
  format: yaml
  label: Afero Cloud OTA Firmware API
  slug: ota-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afero/refs/heads/main/openapi/afero-ota-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: afero.io
  spf: true
- caa:
  - 0 issue " amazontrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: false
  dnssec: false
  domain: readthedocs.io
  spf: false
hosts:
- cert_expires: Sep 28 02:07:36 2026 GMT
  host: www.afero.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 13:31:53 2026 GMT
  host: afero-docs.readthedocs.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: api.afero.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Afero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Afero, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Afero
provider_slug: afero
slug: afero-domain-security
source_filename: afero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.afero.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 02:07:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: afero-docs.readthedocs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 13:31:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.afero.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: afero.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: readthedocs.io\n  dnssec: false\n  caa:\n  - 0 issue \" amazontrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/afero/refs/heads/main/security/afero-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Internet of Things
- IoT Platform
- Connected Devices
- Device Management
- Firmware
- Over-the-Air Updates
- Bluetooth Low Energy
- Embedded Security
- Hardware
---
