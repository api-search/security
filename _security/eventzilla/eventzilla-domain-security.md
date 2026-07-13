---
api_specs:
- filename: openapi.yml
  format: yaml
  label: Eventzilla API
  slug: eventzilla-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventzilla/refs/heads/main/openapi/openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: eventzilla.net
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: eventzillaapi.net
  spf: false
hosts:
- cert_expires: Feb  8 23:59:59 2027 GMT
  host: developer.eventzilla.net
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: www.eventzillaapi.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eventzilla Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eventzilla, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Eventzilla
provider_slug: eventzilla
slug: eventzilla-domain-security
source_filename: eventzilla-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.eventzilla.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  8 23:59:59 2027 GMT\n  hsts: false\n- host: www.eventzillaapi.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: eventzilla.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: eventzillaapi.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eventzilla/refs/heads/main/security/eventzilla-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Events
- Ticketing
- Registration
- Attendees
- Event Management
---
