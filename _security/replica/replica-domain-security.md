---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: replicahq.com
  spf: true
hosts:
- cert_expires: Oct 10 13:31:47 2026 GMT
  host: www.replicahq.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 18:16:35 2026 GMT
  host: documentation.replicahq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: ReadMe.io-hosted data documentation
  tls_version: TLSv1.3
- cert_expires: Sep  8 19:12:40 2026 GMT
  host: help.replicahq.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15552000
  hsts_preload: true
  https: true
  note: Intercom-hosted help center
  tls_version: TLSv1.3
- cert_expires: Sep 14 04:32:06 2026 GMT
  host: studio.replicahq.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  note: Replica Studio application (authenticated)
  tls_version: TLSv1.3
- cert_expires: Sep 16 02:23:41 2026 GMT
  host: api.studio.replicahq.com
  hsts: false
  https: true
  note: private session-authenticated backend for Replica Studio; not a published developer API
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Replica Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Replica, probed live across 5 host(s) and 1 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Replica
provider_slug: replica
slug: replica-domain-security
source_filename: replica-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.replicahq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 13:31:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: documentation.replicahq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 18:16:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: ReadMe.io-hosted data documentation\n- host: help.replicahq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 19:12:40 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  note: Intercom-hosted help center\n- host: studio.replicahq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 04:32:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  note: Replica Studio application (authenticated)\n- host: api.studio.replicahq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires:\
  \ Sep 16 02:23:41 2026 GMT\n  hsts: false\n  note: private session-authenticated backend for Replica Studio; not a published\n    developer API\ndomains:\n- domain: replicahq.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/replica/refs/heads/main/security/replica-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Data
- Mobility
- Transportation
- Geospatial
- Urban Planning
- Travel Demand Modeling
- Government
- Analytics
- Data Platform
---
