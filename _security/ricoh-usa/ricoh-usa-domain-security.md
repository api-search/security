---
api_specs:
- filename: theta-web-api-openapi.yml
  format: yaml
  label: RICOH THETA Web API
  slug: theta-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ricoh-usa/refs/heads/main/openapi/theta-web-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ricoh-usa.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ricoh360.com
  spf: true
hosts:
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: www.ricoh-usa.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 19:28:48 2026 GMT
  host: docs-theta-api.ricoh360.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: 192.168.1.1
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate in certificate chain (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Ricoh Usa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ricoh USA, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ricoh USA
provider_slug: ricoh-usa
slug: ricoh-usa-domain-security
source_filename: ricoh-usa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ricoh-usa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs-theta-api.ricoh360.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 19:28:48 2026 GMT\n  hsts: false\n- host: 192.168.1.1\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate\n    in certificate chain (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: ricoh-usa.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: ricoh360.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ricoh-usa/refs/heads/main/security/ricoh-usa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Printing
- Document Management
- Workplace Services
- Imaging
- 360 Cameras
- Workflow Automation
---
