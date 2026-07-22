---
api_specs:
- filename: vectorsolutions-targetsolutions-openapi.yml
  format: yaml
  label: TargetSolutions API
  slug: targetsolutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorsolutions/refs/heads/main/openapi/vectorsolutions-targetsolutions-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vectorsolutions.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: targetsolutions.com
  spf: true
hosts:
- cert_expires: Sep 14 05:45:54 2026 GMT
  host: vectorsolutions.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: developers.targetsolutions.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: api.targetsolutions.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Vectorsolutions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vector Solutions, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vector Solutions
provider_slug: vectorsolutions
slug: vectorsolutions-domain-security
source_filename: vectorsolutions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vectorsolutions.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 05:45:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.targetsolutions.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: false\n- host: api.targetsolutions.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: vectorsolutions.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: targetsolutions.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vectorsolutions/refs/heads/main/security/vectorsolutions-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Training
- Learning Management
- Compliance
- Public Safety
- Workforce Management
- EHS
- Education
---
