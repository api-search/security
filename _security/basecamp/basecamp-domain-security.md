---
api_specs:
- filename: basecamp-api-openapi.yml
  format: yaml
  label: Basecamp API
  slug: basecamp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/openapi/basecamp-api-openapi.yml
- filename: basecamp-webhooks-asyncapi.yml
  format: yaml
  label: Basecamp Webhooks
  slug: basecamp-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/asyncapi/basecamp-webhooks-asyncapi.yml
- filename: basecamp-oauth-openapi.yml
  format: yaml
  label: Basecamp OAuth
  slug: basecamp-oauth
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/openapi/basecamp-oauth-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:sysadmins@37signals.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: basecamp.com
  spf: true
- caa:
  - 0 iodef "mailto:sysadmins@37signals.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: false
  dnssec: false
  domain: basecampapi.com
  spf: false
hosts:
- cert_expires: Oct  6 06:03:30 2026 GMT
  host: basecamp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 06:20:30 2026 GMT
  host: 3.basecampapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 08:30:05 2026 GMT
  host: launchpad.37signals.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Basecamp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Basecamp, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Basecamp
provider_slug: basecamp
slug: basecamp-domain-security
source_filename: basecamp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: basecamp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 06:03:30 2026 GMT\n  hsts: false\n- host: 3.basecampapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 06:20:30 2026 GMT\n  hsts: false\n- host: launchpad.37signals.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 08:30:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: basecamp.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:sysadmins@37signals.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: basecampapi.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:sysadmins@37signals.com\"\n  - 0 issue \"amazon.com\"\
  \n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/security/basecamp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
---
