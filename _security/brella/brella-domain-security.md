---
api_specs:
- filename: brella-openapi.yml
  format: yaml
  label: Brella Events API
  slug: brella-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brella/refs/heads/main/openapi/brella-openapi.yml
- filename: brella-openapi.yml
  format: yaml
  label: Brella Attendees API
  slug: brella-attendees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brella/refs/heads/main/openapi/brella-openapi.yml
- filename: brella-openapi.yml
  format: yaml
  label: Brella Speakers API
  slug: brella-speakers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brella/refs/heads/main/openapi/brella-openapi.yml
- filename: brella-openapi.yml
  format: yaml
  label: Brella Sponsors API
  slug: brella-sponsors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brella/refs/heads/main/openapi/brella-openapi.yml
- filename: brella-openapi.yml
  format: yaml
  label: Brella Schedule API
  slug: brella-schedule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brella/refs/heads/main/openapi/brella-openapi.yml
- filename: brella-openapi.yml
  format: yaml
  label: Brella Invites API
  slug: brella-invites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brella/refs/heads/main/openapi/brella-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: brella.io
  spf: true
  spf_record: v=spf1 include:spf.mandrillapp.com include:_spf.google.com include:2090809.spf08.hubspotemail.net -all
hosts:
- cert_expires: Oct  7 21:12:23 2026 GMT
  cert_issuer: Google Trust Services (WE1)
  host: api.brella.io
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  https: true
  server: cloudflare
  tls_version: TLSv1.3
- cert_expires: Aug 22 07:45:12 2026 GMT
  cert_issuer: Google Trust Services (WE1)
  host: developer.brella.io
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  server: cloudflare
  tls_version: TLSv1.3
- cert_expires: Aug 20 19:40:44 2026 GMT
  cert_issuer: Google Trust Services (WE1)
  host: www.brella.io
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 31536000
  https: true
  server: cloudflare
  tls_version: TLSv1.3
- cert_expires: Oct  8 05:50:27 2026 GMT
  cert_issuer: Google Trust Services (WE1)
  host: brella.io
  https: true
  redirects_to: https://www.brella.io/
  server: cloudflare
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brella Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brella, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Brella
provider_slug: brella
slug: brella-domain-security
source_filename: brella-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.brella.io\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Google Trust Services (WE1)\n  cert_expires: Oct  7 21:12:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  server: cloudflare\n- host: developer.brella.io\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Google Trust Services (WE1)\n  cert_expires: Aug 22 07:45:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  server: cloudflare\n- host: www.brella.io\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Google Trust Services (WE1)\n  cert_expires: Aug 20 19:40:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: false\n  server: cloudflare\n- host: brella.io\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Google Trust Services (WE1)\n  cert_expires: Oct  8 05:50:27 2026 GMT\n\
  \  redirects_to: https://www.brella.io/\n  server: cloudflare\ndomains:\n- domain: brella.io\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  spf_record: v=spf1 include:spf.mandrillapp.com include:_spf.google.com include:2090809.spf08.hubspotemail.net -all\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brella/refs/heads/main/security/brella-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Events
- Event Networking
- Matchmaking
- Event Platform
- Attendees
- Engagement
- Conferences
- SaaS
---
