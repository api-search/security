---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: locallogic.co
  spf: true
hosts:
- cert_expires: Sep 30 04:02:56 2026 GMT
  host: locallogic.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 19:19:36 2026 GMT
  host: docs.locallogic.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: api.locallogic.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Local Logic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Local Logic, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Local Logic
provider_slug: local-logic
slug: local-logic-domain-security
source_filename: local-logic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: locallogic.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 04:02:56 2026 GMT\n  hsts: false\n- host: docs.locallogic.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 19:19:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.locallogic.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: locallogic.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/local-logic/refs/heads/main/security/local-logic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Location Intelligence
- Real Estate
- Geospatial
- Neighborhoods
- Demographics
- Points of Interest
- Proptech
- Climate Risk
- Location Scores
---
