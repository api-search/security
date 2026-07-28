---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nyiso.com
  spf: true
hosts:
- cert_expires: Nov  8 11:51:20 2026 GMT
  host: www.nyiso.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 13:31:01 2026 GMT
  host: mis.nyiso.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 12:41:13 2026 GMT
  host: oasis.nyiso.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 12:41:13 2026 GMT
  host: api.nyiso.com
  hsts: false
  https: true
  note: Added by hand on 2026-07-27 - the script probes apis.yml Website/Portal and OpenAPI servers[] hosts, and this repo has no OpenAPI, so the API hosts were not covered. Anonymous root returns 404; all documented endpoints return 401.
  server: awselb/2.0
  tls_version: TLSv1.3
  tls_versions_accepted:
  - TLSv1.2
  - TLSv1.3
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: apitest.nyiso.com
  hsts: false
  https: true
  note: Market-trial environment; hand-probed 2026-07-27.
  server: awselb/2.0
  tls_version: TLSv1.3
  tls_versions_accepted:
  - TLSv1.2
  - TLSv1.3
- cert_expires: Sep 23 12:41:13 2026 GMT
  host: oasis-postings.nyiso.com
  hsts: false
  https: true
  note: Hand-probed 2026-07-27; anonymous ListBucket returns 200 application/xml.
  server: AmazonS3
  tls_version: TLSv1.3
  tls_versions_accepted:
  - TLSv1.2
  - TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nyiso Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for New York Independent System Operator (NYISO), probed live across 6 host(s) and 1 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: New York Independent System Operator (NYISO)
provider_slug: nyiso
slug: nyiso-domain-security
source_filename: nyiso-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nyiso.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 11:51:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: mis.nyiso.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 13:31:01 2026 GMT\n  hsts: false\n- host: oasis.nyiso.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 12:41:13 2026 GMT\n  hsts: false\n- host: api.nyiso.com\n  https: true\n  tls_version: TLSv1.3\n  tls_versions_accepted: [TLSv1.2, TLSv1.3]\n  cert_expires: Sep 23 12:41:13 2026 GMT\n  hsts: false\n  server: awselb/2.0\n  note: >-\n    Added by hand on 2026-07-27 - the script probes apis.yml Website/Portal and\n    OpenAPI servers[] hosts, and this repo has no OpenAPI, so the API hosts were\n    not covered. Anonymous root returns 404; all documented endpoints return 401.\n- host: apitest.nyiso.com\n  https: true\n  tls_version:\
  \ TLSv1.3\n  tls_versions_accepted: [TLSv1.2, TLSv1.3]\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: false\n  server: awselb/2.0\n  note: Market-trial environment; hand-probed 2026-07-27.\n- host: oasis-postings.nyiso.com\n  https: true\n  tls_version: TLSv1.3\n  tls_versions_accepted: [TLSv1.2, TLSv1.3]\n  cert_expires: Sep 23 12:41:13 2026 GMT\n  hsts: false\n  server: AmazonS3\n  note: Hand-probed 2026-07-27; anonymous ListBucket returns 200 application/xml.\ndomains:\n- domain: nyiso.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nyiso/refs/heads/main/security/nyiso-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- United States
- Electricity
- Energy Markets
- Grid
- Open Data
- System Operator
- New York
- Renewables
- Emissions
---
