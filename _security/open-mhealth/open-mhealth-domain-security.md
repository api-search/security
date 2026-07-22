---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: openmhealth.org
  spf: true
hosts:
- cert_expires: Sep  3 00:14:52 2026 GMT
  host: www.openmhealth.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Mhealth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open mHealth, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Open mHealth
provider_slug: open-mhealth
slug: open-mhealth-domain-security
source_filename: open-mhealth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.openmhealth.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 00:14:52 2026 GMT\n  hsts: false\ndomains:\n- domain: openmhealth.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-mhealth/refs/heads/main/security/open-mhealth-domain-security.yml
summary_line: TLSv1.3
tags:
- Health
- Healthcare
- Mobile Health
- mHealth
- Digital Health
- Health Data
- Patient Generated Health Data
- Wearables
- Fitness
- Interoperability
- Open Standards
- Open Source
- JSON Schema
- IEEE 1752
- FHIR
- HealthKit
- Nonprofit
---
