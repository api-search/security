---
api_specs:
- filename: liveintent-audiences-openapi.yml
  format: yaml
  label: LiveIntent Audiences API
  slug: audiences
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liveintent/refs/heads/main/openapi/liveintent-audiences-openapi.yml
- filename: liveintent-privacy-openapi.yml
  format: yaml
  label: LiveIntent Privacy Management API
  slug: privacy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liveintent/refs/heads/main/openapi/liveintent-privacy-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: liveintent.com
  spf: true
hosts:
- cert_expires: Sep 16 14:17:34 2026 GMT
  host: www.liveintent.com
  hsts: true
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: audiences-staging.bln.liveintent.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: audiences.liveintent.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Liveintent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LiveIntent, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: LiveIntent
provider_slug: liveintent
slug: liveintent-domain-security
source_filename: liveintent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.liveintent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 14:17:34 2026 GMT\n  hsts: true\n- host: audiences-staging.bln.liveintent.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: null\n- host: audiences.liveintent.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: liveintent.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liveintent/refs/heads/main/security/liveintent-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- AdTech
- Identity
- Email Marketing
- Audience
- Publishers
- Marketers
- Data
---
