---
api_specs:
- filename: xrhealth-platform-openapi.yml
  format: yaml
  label: XRHealth Platform API
  slug: xrhealth-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xrhealth/refs/heads/main/openapi/xrhealth-platform-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: xr.health
  spf: true
hosts:
- cert_expires: Oct 16 07:54:08 2026 GMT
  host: www.xr.health
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 23 06:01:56 2026 GMT
  host: developer.xr.health
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: api.xr.health
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Xrhealth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for XRHealth, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: XRHealth
provider_slug: xrhealth
slug: xrhealth-domain-security
source_filename: xrhealth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.xr.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 07:54:08 2026 GMT\n  hsts: false\n- host: developer.xr.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 06:01:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.xr.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: xr.health\n  dnssec: true\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xrhealth/refs/heads/main/security/xrhealth-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Health
- Digital Health
- Telehealth
- Virtual Reality
- Extended Reality
- Medical Devices
- Rehabilitation
- Mental Health
- Patient Authentication
- Healthcare
---
