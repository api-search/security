---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: landbase.com
  spf: true
hosts:
- cert_expires: Oct 10 03:37:27 2026 GMT
  host: www.landbase.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 23:18:08 2026 GMT
  host: api.landbase.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Landbase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Landbase, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Landbase
provider_slug: landbase
slug: landbase-domain-security
source_filename: landbase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.landbase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 03:37:27 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.landbase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 23:18:08 2026 GMT\n  hsts: null\ndomains:\n- domain: landbase.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/landbase/refs/heads/main/security/landbase-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Go To Market
- Sales
- Marketing
- B2B Data
- Data Enrichment
- Artificial Intelligence
- Agents
- Command Line Interface
- Lead Generation
---
