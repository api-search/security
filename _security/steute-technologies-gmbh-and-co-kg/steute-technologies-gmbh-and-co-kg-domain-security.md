---
api_specs:
- filename: steute-technologies-gmbh-and-co-kg-access-point-api-openapi.yml
  format: yaml
  label: steute Technologies GmbH & Co. KG Access Point API
  slug: steute-technologies-gmbh-and-co-kg-access-point-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/steute-technologies-gmbh-and-co-kg/refs/heads/main/openapi/steute-technologies-gmbh-and-co-kg-access-point-api-openapi.yml
- filename: steute-technologies-gmbh-and-co-kg-auth-api-openapi.yml
  format: yaml
  label: steute Technologies GmbH & Co. KG Auth API
  slug: steute-technologies-gmbh-and-co-kg-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/steute-technologies-gmbh-and-co-kg/refs/heads/main/openapi/steute-technologies-gmbh-and-co-kg-auth-api-openapi.yml
- filename: steute-technologies-gmbh-and-co-kg-history-api-openapi.yml
  format: yaml
  label: steute Technologies GmbH & Co. KG History API
  slug: steute-technologies-gmbh-and-co-kg-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/steute-technologies-gmbh-and-co-kg/refs/heads/main/openapi/steute-technologies-gmbh-and-co-kg-history-api-openapi.yml
- filename: steute-technologies-gmbh-and-co-kg-notification-config-api-openapi.yml
  format: yaml
  label: steute Technologies GmbH & Co. KG Notification Config API
  slug: steute-technologies-gmbh-and-co-kg-notification-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/steute-technologies-gmbh-and-co-kg/refs/heads/main/openapi/steute-technologies-gmbh-and-co-kg-notification-config-api-openapi.yml
- filename: steute-technologies-gmbh-and-co-kg-switch-api-openapi.yml
  format: yaml
  label: steute Technologies GmbH & Co. KG Switch API
  slug: steute-technologies-gmbh-and-co-kg-switch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/steute-technologies-gmbh-and-co-kg/refs/heads/main/openapi/steute-technologies-gmbh-and-co-kg-switch-api-openapi.yml
- filename: steute-technologies-gmbh-and-co-kg-switch-group-api-openapi.yml
  format: yaml
  label: steute Technologies GmbH & Co. KG Switch Group API
  slug: steute-technologies-gmbh-and-co-kg-switch-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/steute-technologies-gmbh-and-co-kg/refs/heads/main/openapi/steute-technologies-gmbh-and-co-kg-switch-group-api-openapi.yml
- filename: steute-technologies-gmbh-and-co-kg-system-status-api-openapi.yml
  format: yaml
  label: steute Technologies GmbH & Co. KG System Status API
  slug: steute-technologies-gmbh-and-co-kg-system-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/steute-technologies-gmbh-and-co-kg/refs/heads/main/openapi/steute-technologies-gmbh-and-co-kg-system-status-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: steute.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: nexy.net
  spf: false
hosts:
- cert_expires: Oct  7 18:13:45 2026 GMT
  host: www.steute.com
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 23:18:03 2026 GMT
  host: docs.nexy.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: 192.168.3.32
  https: false
kind: domain-security
layout: security
method: probed
name: Steute Technologies Gmbh And Co Kg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for steute Technologies GmbH & Co. KG, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: steute Technologies GmbH & Co. KG
provider_slug: steute-technologies-gmbh-and-co-kg
slug: steute-technologies-gmbh-and-co-kg-domain-security
source_filename: steute-technologies-gmbh-and-co-kg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.steute.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 18:13:45 2026 GMT\n  hsts: true\n  hsts_max_age: 16070400\n- host: docs.nexy.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 23:18:03 2026 GMT\n  hsts: false\n- host: 192.168.3.32\n  https: false\ndomains:\n- domain: steute.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: nexy.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/steute-technologies-gmbh-and-co-kg/refs/heads/main/security/steute-technologies-gmbh-and-co-kg-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Industrial
- Manufacturing
- IIoT
- Wireless
- Sensors
- Switches
- Intralogistics
- Automation
- Medical Devices
---
