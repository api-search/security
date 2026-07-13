---
api_specs:
- filename: callrail-openapi.yml
  format: yaml
  label: CallRail v3 API
  slug: v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/callrail/refs/heads/main/openapi/callrail-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: callrail.com
  spf: true
hosts:
- cert_expires: Aug 21 01:33:48 2026 GMT
  host: www.callrail.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 21:05:18 2026 GMT
  host: apidocs.callrail.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 23:59:59 2026 GMT
  host: api.callrail.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Callrail Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CallRail, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CallRail
provider_slug: callrail
slug: callrail-domain-security
source_filename: callrail-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.callrail.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 01:33:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apidocs.callrail.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 21:05:18 2026 GMT\n  hsts: false\n- host: api.callrail.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 15 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: callrail.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/callrail/refs/heads/main/security/callrail-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Call Tracking
- Conversation Intelligence
- Marketing Attribution
- Lead Tracking
- Telephony
- Analytics
- Form Tracking
---
