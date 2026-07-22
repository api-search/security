---
api_specs:
- filename: quo-public-api-v1.json
  format: json
  label: Quo Public API
  slug: quo-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quo/refs/heads/main/openapi/quo-public-api-v1.json
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: quo.com
  spf: true
hosts:
- cert_expires: Oct 14 23:02:21 2026 GMT
  host: quo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 05:54:28 2026 GMT
  host: api.quo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quo, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Quo
provider_slug: quo
slug: quo-domain-security
source_filename: quo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:02:21 2026 GMT\n  hsts: false\n- host: api.quo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 05:54:28 2026 GMT\n  hsts: null\ndomains:\n- domain: quo.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quo/refs/heads/main/security/quo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Communication
- Messaging
- SMS
- Voice
- Contacts
- Webhooks
- API
---
