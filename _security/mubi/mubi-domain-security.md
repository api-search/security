---
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:abuse@mubi.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mubi.com
  spf: true
hosts:
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: mubi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: api.mubi.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  note: undocumented first-party client API host; root returns 404
  tls_version: TLSv1.2
- cert_expires: Sep 24 16:10:35 2026 GMT
  host: help.mubi.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mubi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MUBI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MUBI
provider_slug: mubi
slug: mubi-domain-security
source_filename: mubi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mubi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.mubi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n  note: undocumented first-party client API host; root returns 404\n- host: help.mubi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 16:10:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\ndomains:\n- domain: mubi.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:abuse@mubi.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mubi/refs/heads/main/security/mubi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Streaming
- Media
- Entertainment
- Film
- Video On Demand
- Subscription
- Distribution
---
