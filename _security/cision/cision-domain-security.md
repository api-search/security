---
api_specs:
- filename: openapi.yml
  format: yaml
  label: CisionOne API
  slug: cisionone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cision/refs/heads/main/openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cision.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cision.one
  spf: true
hosts:
- cert_expires: Sep 20 07:33:52 2026 GMT
  host: www.cision.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 11:07:05 2026 GMT
  host: api.cision.one
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cision Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cision, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cision
provider_slug: cision
slug: cision-domain-security
source_filename: cision-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cision.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 07:33:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.cision.one\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 11:07:05 2026 GMT\n  hsts: null\ndomains:\n- domain: cision.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: cision.one\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cision/refs/heads/main/security/cision-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- PR Software
- Public Relations
- Earned Media
- Media Monitoring
- Press Release Distribution
- Media Database
- Influencer Identification
- Analytics
---
