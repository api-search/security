---
api_specs:
- filename: accruent-maintenance-connection-openapi.yml
  format: yaml
  label: Maintenance Connection Web API
  slug: maintenance-connection-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accruent/refs/heads/main/openapi/accruent-maintenance-connection-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: accruent.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: maintenanceconnection.com
  spf: true
hosts:
- cert_expires: Nov 21 06:55:20 2026 GMT
  host: www.accruent.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 25 06:46:41 2026 GMT
  host: api.maintenanceconnection.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  5 05:00:33 2026 GMT
  host: developer.accruent.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Accruent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Accruent, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Accruent
provider_slug: accruent
slug: accruent-domain-security
source_filename: accruent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.accruent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 06:55:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.maintenanceconnection.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 06:46:41 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developer.accruent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 05:00:33 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: accruent.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: maintenanceconnection.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accruent/refs/heads/main/security/accruent-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Facilities Management
- Asset Management
- CMMS
- EAM
- Maintenance
- Work Orders
- IWMS
- Space Management
- Engineering Document Management
- Built Environment
- Enterprise Software
- Real Estate
---
