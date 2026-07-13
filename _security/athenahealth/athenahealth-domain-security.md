---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: athenahealth.com
  spf: true
hosts:
- cert_expires: Aug 17 17:23:46 2026 GMT
  host: www.athenahealth.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 12 23:59:59 2027 GMT
  host: docs.athenahealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.athenahealth.com
  https: false
kind: domain-security
layout: security
method: probed
name: Athenahealth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for athenahealth, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: athenahealth
provider_slug: athenahealth
slug: athenahealth-domain-security
source_filename: athenahealth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.athenahealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 17:23:46 2026 GMT\n  hsts: null\n- host: docs.athenahealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 23:59:59 2027 GMT\n  hsts: false\n- host: api.athenahealth.com\n  https: false\ndomains:\n- domain: athenahealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/athenahealth/refs/heads/main/security/athenahealth-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Healthcare
- EHR
- Electronic Health Records
- Practice Management
- Revenue Cycle Management
- Patient Portal
- FHIR
- Care Coordination
- Interoperability
- HL7
---
