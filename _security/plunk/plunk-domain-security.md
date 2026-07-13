---
api_specs:
- filename: plunk-openapi.yml
  format: yaml
  label: Plunk Send (Transactional) API
  slug: plunk-send-transactional-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plunk/refs/heads/main/openapi/plunk-openapi.yml
- filename: plunk-openapi.yml
  format: yaml
  label: Plunk Track (Events) API
  slug: plunk-track-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plunk/refs/heads/main/openapi/plunk-openapi.yml
- filename: plunk-openapi.yml
  format: yaml
  label: Plunk Contacts API
  slug: plunk-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plunk/refs/heads/main/openapi/plunk-openapi.yml
- filename: plunk-openapi.yml
  format: yaml
  label: Plunk Campaigns API
  slug: plunk-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plunk/refs/heads/main/openapi/plunk-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: useplunk.com
  spf: true
hosts:
- cert_expires: Oct  4 09:04:51 2026 GMT
  host: www.useplunk.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 09:04:59 2026 GMT
  host: docs.useplunk.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 05:07:21 2026 GMT
  host: api.useplunk.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Plunk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Plunk, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Plunk
provider_slug: plunk
slug: plunk-domain-security
source_filename: plunk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.useplunk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 09:04:51 2026 GMT\n  hsts: false\n- host: docs.useplunk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 09:04:59 2026 GMT\n  hsts: false\n- host: api.useplunk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 05:07:21 2026 GMT\n  hsts: false\ndomains:\n- domain: useplunk.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plunk/refs/heads/main/security/plunk-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Email
- Transactional Email
- Marketing
- Automation
- Open Source
- SaaS
---
