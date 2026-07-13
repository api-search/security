---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: netsmartcloud.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ntst.com
  spf: true
hosts:
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: careconnect.netsmartcloud.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: fhir.netsmartcloud.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: www.ntst.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Netsmart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Netsmart, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Netsmart
provider_slug: netsmart
slug: netsmart-domain-security
source_filename: netsmart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: careconnect.netsmartcloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: false\n- host: fhir.netsmartcloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: false\n- host: www.ntst.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: netsmartcloud.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: ntst.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/netsmart/refs/heads/main/security/netsmart-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare IT
- EHR
- FHIR
- Behavioral Health
- Post-Acute Care
- Human Services
- Interoperability
- HL7
- Care Coordination
---
