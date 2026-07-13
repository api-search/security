---
api_specs:
- filename: zoominfo-openapi.yml
  format: yaml
  label: ZoomInfo
  slug: zoominfo
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/openapi/zoominfo-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:security@zoominfo.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "entrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zoominfo.com
  spf: true
hosts:
- cert_expires: Sep 23 16:29:49 2026 GMT
  host: www.zoominfo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 16:29:49 2026 GMT
  host: api.zoominfo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zoominfo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ZoomInfo, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ZoomInfo
provider_slug: zoominfo
slug: zoominfo-domain-security
source_filename: zoominfo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zoominfo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 16:29:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.zoominfo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 16:29:49 2026 GMT\n  hsts: null\ndomains:\n- domain: zoominfo.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:security@zoominfo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"entrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/security/zoominfo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- B2B
- B2B Data
- Company Data
- Contact Database
- Contacts
- Data
- Lead Generation
- Marketing Intelligence
- Sales Intelligence
---
