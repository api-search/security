---
api_specs:
- filename: jb-hunt-360-connect-api.yml
  format: yaml
  label: J.B. Hunt 360 Connect API
  slug: jb-hunt-360-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jb-hunt-transport-services/refs/heads/main/openapi/jb-hunt-360-connect-api.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jbhunt.com
  spf: true
hosts:
- host: apiportal.jbhunt.com
  https: false
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: www.jbhunt.com
  hsts: true
  hsts_max_age: 3600
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: api.jbhunt.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jb Hunt Transport Services Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for J.B. Hunt Transport Services, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: J.B. Hunt Transport Services
provider_slug: jb-hunt-transport-services
slug: jb-hunt-transport-services-domain-security
source_filename: jb-hunt-transport-services-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apiportal.jbhunt.com\n  https: false\n- host: www.jbhunt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 3600\n- host: api.jbhunt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: jbhunt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jb-hunt-transport-services/refs/heads/main/security/jb-hunt-transport-services-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Freight
- Intermodal
- Logistics
- Shipping
- Supply Chain
- Transportation
- Trucking
- Fortune 500
---
