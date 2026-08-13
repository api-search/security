---
api_specs:
- filename: habu-clean-room-api-openapi.yml
  format: yaml
  label: Habu Clean Room API
  slug: habu-clean-room-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/habu/refs/heads/main/openapi/habu-clean-room-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: habu.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: liveramp.com
  spf: true
hosts:
- cert_expires: Oct 18 10:40:03 2026 GMT
  host: habu.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 03:33:14 2026 GMT
  host: developers.liveramp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: api.habu.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Habu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Habu, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Habu
provider_slug: habu
slug: habu-domain-security
source_filename: habu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: habu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 10:40:03 2026 GMT\n  hsts: false\n- host: developers.liveramp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 03:33:14 2026 GMT\n  hsts: false\n- host: api.habu.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: habu.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: liveramp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/habu/refs/heads/main/security/habu-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Data Clean Room
- Data Collaboration
- Advertising
- Privacy
- Identity
- Marketing
- Analytics
---
