---
api_specs:
- filename: missive-rest-api-openapi.yml
  format: yaml
  label: Missive REST API
  slug: missive-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/missive/refs/heads/main/openapi/missive-rest-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: missiveapp.com
  spf: true
hosts:
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: missiveapp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: public.missiveapp.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Missive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Missive, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Missive
provider_slug: missive
slug: missive-domain-security
source_filename: missive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: missiveapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: public.missiveapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: missiveapp.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/missive/refs/heads/main/security/missive-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Team Inbox
- Collaboration
- Email
- Messaging
- Conversations
- Contacts
- Webhooks
- Automation
- REST API
---
