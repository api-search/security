---
api_specs:
- filename: tata-communications-number-intelligence-api.json
  format: json
  label: Number Intelligence API
  slug: tata-communications-number-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tata-communications/refs/heads/main/openapi/tata-communications-number-intelligence-api.json
- filename: tata-communications-mobile-messaging-exchange-account-administration.json
  format: json
  label: Mobile Messaging Exchange - Account Administration
  slug: tata-communications-mobile-messaging-exchange-account-administration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tata-communications/refs/heads/main/openapi/tata-communications-mobile-messaging-exchange-account-administration.json
- filename: tata-communications-mobile-messaging-exchange-cdr-report-api.json
  format: json
  label: Mobile Messaging Exchange - CDR Report API
  slug: tata-communications-mobile-messaging-exchange-cdr-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tata-communications/refs/heads/main/openapi/tata-communications-mobile-messaging-exchange-cdr-report-api.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tatacommunications.com
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: false
  dnssec: false
  domain: azure-api.net
  spf: false
hosts:
- cert_expires: Sep 29 22:14:23 2026 GMT
  host: www.tatacommunications.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: developer.tatacommunications.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov  1 21:14:07 2026 GMT
  host: move-external-apim-prod.developer.azure-api.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tata Communications Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tata Communications, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tata Communications
provider_slug: tata-communications
slug: tata-communications-domain-security
source_filename: tata-communications-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tatacommunications.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 22:14:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.tatacommunications.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: false\n- host: move-external-apim-prod.developer.azure-api.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 21:14:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tatacommunications.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: azure-api.net\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tata-communications/refs/heads/main/security/tata-communications-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Telecommunications
- India
- Wholesale Carrier
- CPaaS
- Messaging
- Voice
- IoT
- eSIM
- Number Intelligence
- Connectivity
- Subsea Cable
- Partner Gated
---
