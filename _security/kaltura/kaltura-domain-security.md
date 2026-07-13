---
api_specs:
- filename: ovp.openapi.json
  format: json
  label: Kaltura VPaaS API
  slug: vpaas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/kaltura/developer-platform/master/ovp.openapi.json
- filename: ott.openapi.json
  format: json
  label: Kaltura OTT Backend API
  slug: ott-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/kaltura/developer-platform/master/ott.openapi.json
description: ''
domains:
- caa:
  - 0 iodef "mailto:security@kaltura.com"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "globalsign.com"
  - 0 issue "ssl.com"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kaltura.com
  spf: true
hosts:
- cert_expires: Sep 14 23:59:59 2026 GMT
  host: corp.kaltura.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  8 06:40:44 2026 GMT
  host: developer.kaltura.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: www.kaltura.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Kaltura Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kaltura, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kaltura
provider_slug: kaltura
slug: kaltura-domain-security
source_filename: kaltura-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: corp.kaltura.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.kaltura.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  8 06:40:44 2026 GMT\n  hsts: false\n- host: www.kaltura.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kaltura.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:security@kaltura.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kaltura/refs/heads/main/security/kaltura-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Video
- Live Streaming
- Transcoding
- Media Management
- Player
- Analytics
- Virtual Classroom
- OTT
- Open Source
---
