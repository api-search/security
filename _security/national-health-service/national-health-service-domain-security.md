---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nhs.uk
  spf: true
hosts:
- cert_expires: Jul 22 23:59:59 2026 GMT
  host: www.nhs.uk
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 21:58:44 2026 GMT
  host: digital.nhs.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: api.service.nhs.uk
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: National Health Service Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Health Service, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: National Health Service
provider_slug: national-health-service
slug: national-health-service-domain-security
source_filename: national-health-service-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nhs.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: digital.nhs.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 21:58:44 2026 GMT\n  hsts: null\n- host: api.service.nhs.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: nhs.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-health-service/refs/heads/main/security/national-health-service-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Ambulance
- Health
- Healthcare
- National Health Service
---
