---
api_specs:
- filename: appbrilliance-ping-api-openapi.yml
  format: yaml
  label: AppBrilliance Ping API
  slug: appbrilliance-ping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appbrilliance/refs/heads/main/openapi/appbrilliance-ping-api-openapi.yml
- filename: appbrilliance-transaction-api-openapi.yml
  format: yaml
  label: AppBrilliance Transaction API
  slug: appbrilliance-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appbrilliance/refs/heads/main/openapi/appbrilliance-transaction-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: appbrilliance.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: securenet.live
  spf: false
hosts:
- cert_expires: Nov  1 19:24:05 2026 GMT
  host: appbrilliance.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 12 20:47:02 2026 GMT
  host: dev.appbrilliance.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov  9 23:59:59 2026 GMT
  host: customer.api.securenet.live
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Appbrilliance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AppBrilliance, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AppBrilliance
provider_slug: appbrilliance
slug: appbrilliance-domain-security
source_filename: appbrilliance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: appbrilliance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 19:24:05 2026 GMT\n  hsts: false\n- host: dev.appbrilliance.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 12 20:47:02 2026 GMT\n  hsts: false\n- host: customer.api.securenet.live\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: appbrilliance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: securenet.live\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appbrilliance/refs/heads/main/security/appbrilliance-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Payments
- Fintech
- Agentic Payments
- Open Banking
- Enterprise
---
