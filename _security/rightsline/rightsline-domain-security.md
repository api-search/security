---
api_specs:
- filename: postman.yaml
  format: yaml
  label: Rightsline Rights API
  slug: rights-api
  spec_type: Postman
  url: https://postman.rightsline.com/
- filename: postman.yaml
  format: yaml
  label: Rightsline Royalties API
  slug: royalties-api
  spec_type: Postman
  url: https://postman.rightsline.com/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rightsline.com
  spf: true
hosts:
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: www.rightsline.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: app.rightsline.com
  hsts: true
  hsts_max_age: 6307200
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 13:30:39 2026 GMT
  host: api-docs.rightsline.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rightsline Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rightsline, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Rightsline
provider_slug: rightsline
slug: rightsline-domain-security
source_filename: rightsline-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rightsline.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.rightsline.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 6307200\n- host: api-docs.rightsline.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 13:30:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rightsline.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rightsline/refs/heads/main/security/rightsline-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Content Management
- Entertainment
- Media
- Rights Management
- Royalties
---
