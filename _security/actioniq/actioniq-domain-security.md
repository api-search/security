---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: actioniq.com
  spf: true
hosts:
- cert_expires: Sep 28 01:03:19 2026 GMT
  host: www.actioniq.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: api.actioniq.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Actioniq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ActionIQ, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ActionIQ
provider_slug: actioniq
slug: actioniq-domain-security
source_filename: actioniq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.actioniq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 01:03:19 2026 GMT\n  hsts: false\n- host: api.actioniq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: actioniq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/actioniq/refs/heads/main/security/actioniq-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Customer Data Platform
- CDP
- Audience Management
- Real-Time Personalization
- Marketing Orchestration
- Data Activation
- Enterprise
- REST API
---
