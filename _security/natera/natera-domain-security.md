---
api_specs:
- filename: natera-openapi.yml
  format: yaml
  label: Natera EMR Ordering and Results Integration
  slug: natera-emr-ordering-integration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natera/refs/heads/main/openapi/natera-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: natera.com
  spf: true
hosts:
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: www.natera.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  6 23:59:59 2027 GMT
  host: constellation.natera.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 21:32:02 2026 GMT
  host: connect.natera.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Natera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Natera, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Natera
provider_slug: natera
slug: natera-domain-security
source_filename: natera-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.natera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: constellation.natera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: connect.natera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 21:32:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: natera.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/natera/refs/heads/main/security/natera-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Genetic Testing
- Healthcare
- Diagnostics
- EHR Integration
- HL7
---
