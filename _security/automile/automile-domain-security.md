---
api_specs:
- filename: automile-openapi-original.json
  format: json
  label: Automile API
  slug: automile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automile/refs/heads/main/openapi/automile-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: automile.com
  spf: true
hosts:
- cert_expires: Oct 14 12:11:48 2026 GMT
  host: www.automile.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Automile Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Automile, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Automile
provider_slug: automile
slug: automile-domain-security
source_filename: automile-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.automile.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 12:11:48 2026 GMT\n  hsts: false\ndomains:\n- domain: automile.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/automile/refs/heads/main/security/automile-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Fleet Management
- Telematics
- GPS Tracking
- Vehicles
- Transportation
- Mileage
- IoT
- Logistics
- Company
---
