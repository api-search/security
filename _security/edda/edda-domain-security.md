---
api_specs:
- filename: edda-wordpress-openapi.yml
  format: yaml
  label: EDDA Technology WordPress REST API
  slug: wordpress
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edda/refs/heads/main/openapi/edda-wordpress-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: eddatech.com
  spf: true
hosts:
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: www.eddatech.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Edda Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EDDA Technology, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: EDDA Technology
provider_slug: edda
slug: edda-domain-security
source_filename: edda-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eddatech.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: eddatech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edda/refs/heads/main/security/edda-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Health Tech
- Medical Imaging
- Radiology
- Surgery
- Oncology
- Artificial Intelligence
- Medical Devices
- Healthcare
- Clinical Software
---
