---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cloudwell.io
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
hosts:
- cert_expires: Oct  2 06:22:24 2026 GMT
  host: cloudwell.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: appsource.microsoft.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 02:26:09 2026 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cloudwell Opal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cloudwell, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cloudwell
provider_slug: cloudwell-opal
slug: cloudwell-opal-domain-security
source_filename: cloudwell-opal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cloudwell.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 06:22:24 2026 GMT\n  hsts: false\n- host: appsource.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: null\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cloudwell.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudwell-opal/refs/heads/main/security/cloudwell-opal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AppSource
- Calendar Overlay
- Microsoft 365
- Microsoft Partner
- Org Chart
- SharePoint
- SPFx
- Staff Directory
- Teams
- Viva Connections
---
