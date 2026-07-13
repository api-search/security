---
api_specs:
- filename: teledyne-flir-camera-rest-openapi.yml
  format: yaml
  label: Teledyne FLIR Camera REST API
  slug: flir-camera-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teledyne-technologies/refs/heads/main/openapi/teledyne-flir-camera-rest-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: teledyne.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: teledynelecroy.com
  spf: true
hosts:
- cert_expires: Sep  4 15:58:22 2026 GMT
  host: www.teledyne.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 22:34:51 2026 GMT
  host: www.teledynelecroy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 18:02:10 2026 GMT
  host: www.teledyneimaging.com
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Teledyne Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Teledyne Technologies, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Teledyne Technologies
provider_slug: teledyne-technologies
slug: teledyne-technologies-domain-security
source_filename: teledyne-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.teledyne.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 15:58:22 2026 GMT\n  hsts: false\n- host: www.teledynelecroy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 22:34:51 2026 GMT\n  hsts: null\n- host: www.teledyneimaging.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 11 18:02:10 2026 GMT\n  hsts: true\n  hsts_max_age: 10886400\ndomains:\n- domain: teledyne.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: teledynelecroy.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teledyne-technologies/refs/heads/main/security/teledyne-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Aerospace
- Defense
- Digital Imaging
- Instrumentation
- Thermal Imaging
- Test and Measurement
- Fortune 500
---
