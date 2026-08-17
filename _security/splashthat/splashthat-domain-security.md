---
api_specs:
- filename: splashthat-api.postman_collection.json
  format: json
  label: Splash API
  slug: splash-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/splashthat/refs/heads/main/postman/splashthat-api.postman_collection.json
description: ''
domains:
- caa:
  - 0 iodef "mailto:security@splashthat.com"
  - 0 issue "amazon.com"
  - 0 issue "certainly.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: splashthat.com
  spf: true
hosts:
- cert_expires: Oct 21 04:10:15 2026 GMT
  host: api-docs.splashthat.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 02:23:08 2026 GMT
  host: api.splashthat.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Splashthat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Splash, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Splash
provider_slug: splashthat
slug: splashthat-domain-security
source_filename: splashthat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api-docs.splashthat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 04:10:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.splashthat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 02:23:08 2026 GMT\n  hsts: null\ndomains:\n- domain: splashthat.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:security@splashthat.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/splashthat/refs/heads/main/security/splashthat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Events
- Event Marketing
- Event Management
- Guest Registration
- Ticketing
- Check-In
- Analytics
---
