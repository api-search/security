---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: embeddable.com
  spf: true
hosts:
- cert_expires: Sep 28 17:54:49 2026 GMT
  host: embeddable.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 10:46:05 2026 GMT
  host: docs.embeddable.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 05:24:03 2026 GMT
  host: api.us.embeddable.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Embeddable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Embeddable, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Embeddable
provider_slug: embeddable
slug: embeddable-domain-security
source_filename: embeddable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: embeddable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 17:54:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.embeddable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 10:46:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.us.embeddable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 05:24:03 2026 GMT\n  hsts: null\ndomains:\n- domain: embeddable.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/embeddable/refs/heads/main/security/embeddable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Analytics
- Embedded Analytics
- Business Intelligence
- Dashboards
- Data Visualization
- Semantic Layer
- Developer Tools
- SaaS
---
