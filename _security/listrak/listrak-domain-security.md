---
api_specs:
- filename: listrak-email-openapi.yml
  format: yaml
  label: Listrak Email REST API
  slug: email
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listrak/refs/heads/main/openapi/listrak-email-openapi.yml
- filename: listrak-sms-openapi.yml
  format: yaml
  label: Listrak SMS REST API
  slug: sms
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listrak/refs/heads/main/openapi/listrak-sms-openapi.yml
- filename: listrak-crosschannel-openapi.yml
  format: yaml
  label: Listrak Cross Channel REST API
  slug: crosschannel
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listrak/refs/heads/main/openapi/listrak-crosschannel-openapi.yml
- filename: listrak-data-openapi.yml
  format: yaml
  label: Listrak Data Import REST API
  slug: data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listrak/refs/heads/main/openapi/listrak-data-openapi.yml
- filename: listrak-twowaysms-openapi.yml
  format: yaml
  label: Listrak Two-Way SMS Conversation REST API
  slug: twowaysms
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listrak/refs/heads/main/openapi/listrak-twowaysms-openapi.yml
- filename: listrak-mobileclient-openapi.yml
  format: yaml
  label: Listrak Mobile App Push API
  slug: mobileclient
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listrak/refs/heads/main/openapi/listrak-mobileclient-openapi.yml
- filename: listrak-privacy-openapi.yml
  format: yaml
  label: Listrak Privacy REST API
  slug: privacy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listrak/refs/heads/main/openapi/listrak-privacy-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "cloudflare.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: listrak.com
  spf: true
hosts:
- cert_expires: Aug 16 10:09:40 2026 GMT
  host: www.listrak.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 19:02:39 2026 GMT
  host: api.listrak.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Listrak Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Listrak, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Listrak
provider_slug: listrak
slug: listrak-domain-security
source_filename: listrak-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.listrak.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 10:09:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.listrak.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 19:02:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: listrak.com\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"cloudflare.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/listrak/refs/heads/main/security/listrak-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email Marketing
- SMS Marketing
- Marketing Automation
- Cross-Channel
- Retail
- Push Notifications
- Data Import
- Privacy
---
