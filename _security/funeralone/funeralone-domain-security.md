---
api_specs:
- filename: funeralone-openapi.yml
  format: yaml
  label: funeralOne Cases API
  slug: funeralone-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/funeralone/refs/heads/main/openapi/funeralone-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: funeralone.com
  spf: true
hosts:
- cert_expires: Aug 17 07:26:06 2026 GMT
  host: www.funeralone.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 07:26:06 2026 GMT
  host: api.funeralone.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Funeralone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for funeralOne, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: funeralOne
provider_slug: funeralone
slug: funeralone-domain-security
source_filename: funeralone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.funeralone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 07:26:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.funeralone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 07:26:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: funeralone.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/funeralone/refs/heads/main/security/funeralone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Funeral Homes
- Deathcare
- Obituaries
- Tribute Videos
- Memorial Websites
- Life Tributes
- Case Management
- Partner API
---
