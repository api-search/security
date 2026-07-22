---
api_specs:
- filename: wunderkind-email-openapi.yml
  format: yaml
  label: Wunderkind Email API
  slug: wunderkind-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wunderkind/refs/heads/main/openapi/wunderkind-email-openapi.yml
- filename: wunderkind-identity-openapi.yml
  format: yaml
  label: Wunderkind Identity API
  slug: wunderkind-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wunderkind/refs/heads/main/openapi/wunderkind-identity-openapi.yml
- filename: wunderkind-ucrm-openapi.yml
  format: yaml
  label: Wunderkind UCRM API
  slug: wunderkind-ucrm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wunderkind/refs/heads/main/openapi/wunderkind-ucrm-openapi.yml
- filename: wunderkind-event-ingestion-openapi.yml
  format: yaml
  label: Wunderkind Event Ingestion API
  slug: wunderkind-event-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wunderkind/refs/heads/main/openapi/wunderkind-event-ingestion-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: wunderkind.co
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: wknd.ai
  spf: false
hosts:
- cert_expires: Sep 16 18:11:16 2026 GMT
  host: www.wunderkind.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 17:30:28 2026 GMT
  host: developer.wunderkind.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 08:01:03 2026 GMT
  host: api.wunderkind.co
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.wknd.ai
  hsts: false
  https: true
  note: Serves HTTP/2 over TLS (404 on /); no Strict-Transport-Security header observed.
  tls_version: null
kind: domain-security
layout: security
method: probed
name: Wunderkind Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wunderkind, probed live across 4 host(s) and 2 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Wunderkind
provider_slug: wunderkind
slug: wunderkind-domain-security
source_filename: wunderkind-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wunderkind.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 18:11:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.wunderkind.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 17:30:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.wunderkind.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 08:01:03 2026 GMT\n  hsts: null\n- host: api.wknd.ai\n  https: true\n  tls_version: null\n  hsts: false\n  note: Serves HTTP/2 over TLS (404 on /); no Strict-Transport-Security header observed.\ndomains:\n- domain: wunderkind.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: wknd.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wunderkind/refs/heads/main/security/wunderkind-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Marketing
- Personalization
- Identity Resolution
- Email
- SMS
- Behavioral Data
- eCommerce
- Webhooks
---
