---
api_specs:
- filename: screenshotone-openapi.yml
  format: yaml
  label: ScreenshotOne API
  slug: screenshotone
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/screenshotone/refs/heads/main/openapi/screenshotone-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: screenshotone.com
  spf: true
hosts:
- cert_expires: Aug 24 15:08:01 2026 GMT
  host: screenshotone.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 19:54:02 2026 GMT
  host: api.screenshotone.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Screenshotone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ScreenshotOne, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ScreenshotOne
provider_slug: screenshotone
slug: screenshotone-domain-security
source_filename: screenshotone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: screenshotone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 15:08:01 2026 GMT\n  hsts: false\n- host: api.screenshotone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 19:54:02 2026 GMT\n  hsts: null\ndomains:\n- domain: screenshotone.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/screenshotone/refs/heads/main/security/screenshotone-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Images
- Screenshots
- Web Rendering
---
