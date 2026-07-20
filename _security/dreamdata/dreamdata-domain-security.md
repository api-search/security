---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dreamdata.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dreamdata.cloud
  spf: true
hosts:
- cert_expires: Oct 13 19:43:19 2026 GMT
  host: dreamdata.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 18:32:18 2026 GMT
  host: developer.dreamdata.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 20:08:36 2026 GMT
  host: api.dreamdata.cloud
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dreamdata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dreamdata, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Dreamdata
provider_slug: dreamdata
slug: dreamdata-domain-security
source_filename: dreamdata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dreamdata.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 19:43:19 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developer.dreamdata.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 18:32:18 2026 GMT\n  hsts: false\n- host: api.dreamdata.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 20:08:36 2026 GMT\n  hsts: null\ndomains:\n- domain: dreamdata.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: dreamdata.cloud\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dreamdata/refs/heads/main/security/dreamdata-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- B2B Attribution
- Revenue Attribution
- Marketing Analytics
- Customer Journey
- Event Tracking
- Audience Activation
- Analytics
- MCP
---
