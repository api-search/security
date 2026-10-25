---
api_specs:
- filename: life360-product-api-openapi.yml
  format: yaml
  label: Life360 Product API
  slug: life360-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/life360/refs/heads/main/openapi/life360-product-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 iodef "mailto:caa-issues@life360.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: life360.com
  spf: true
hosts:
- cert_expires: Dec 29 13:31:32 2026 GMT
  host: www.life360.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Life360 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Life360, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Life360
provider_slug: life360
slug: life360-domain-security
source_filename: life360-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.life360.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 13:31:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: life360.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 iodef \"mailto:caa-issues@life360.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/life360/refs/heads/main/security/life360-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Family Safety
- Location
- GPS Tracking
- Bluetooth Trackers
- Mobile App
- Driving Safety
- Wearables
- Subscription
---
