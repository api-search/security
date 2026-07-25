---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: well.company
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: apps.health
  spf: true
hosts:
- cert_expires: Oct  1 01:42:18 2026 GMT
  host: well.company
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 05:02:29 2026 GMT
  host: apps.health
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Well Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WELL Health Technologies, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: WELL Health Technologies
provider_slug: well-health
slug: well-health-domain-security
source_filename: well-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: well.company\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 01:42:18 2026 GMT\n  hsts: false\n- host: apps.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 05:02:29 2026 GMT\n  hsts: false\ndomains:\n- domain: well.company\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: apps.health\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/well-health/refs/heads/main/security/well-health-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Healthcare
- Canada
- EMR
- EHR
- FHIR
- HL7
- Interoperability
- Digital Health
- Telehealth
- ePharma
- Clinics
---
