---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: medicaldirector.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: telstrahealth.com
  spf: true
hosts:
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: www.medicaldirector.com
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 03:54:03 2026 GMT
  host: www.telstrahealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Medical Director Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MedicalDirector, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MedicalDirector
provider_slug: medical-director
slug: medical-director-domain-security
source_filename: medical-director-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.medicaldirector.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 10886400\n- host: www.telstrahealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 03:54:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: medicaldirector.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: telstrahealth.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medical-director/refs/heads/main/security/medical-director-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Australia
- EHR
- EMR
- FHIR
- Interoperability
- Practice Management
- Primary Care
- Clinical Software
- Digital Health
---
