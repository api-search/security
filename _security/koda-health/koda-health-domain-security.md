---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: kodahealthcare.com
  spf: true
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: true
  domain: koda.health
  spf: false
hosts:
- cert_expires: Sep  5 11:05:05 2026 GMT
  host: www.kodahealthcare.com
  hsts: false
  https: true
  role: marketing site
  tls_version: TLSv1.3
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: app.kodahealthcare.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  notes: Strongest posture of the estate — also sets CSP with report-uri, X-Frame-Options DENY, X-Content-Type-Options nosniff, Cross-Origin-Opener-Policy same-origin, Referrer-Policy no-referrer, and Permissions-Policy denying geolocation/microphone/camera.
  role: patient/provider application (S3 + CloudFront)
- cert_expires: Sep 20 23:59:59 2026 GMT
  host: api.kodahealthcare.com
  hsts: false
  https: true
  role: closed backend API (AWS ELB, awselb/2.0); 403 to all unauthenticated requests
  tls_version: TLSv1.2
- cert_expires: Sep 24 01:04:29 2026 GMT
  host: koda.health
  hsts: false
  https: true
  role: patient-facing marketing site
kind: domain-security
layout: security
method: probed
name: Koda Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Koda Health, probed live across 4 host(s) and 2 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Koda Health
provider_slug: koda-health
slug: koda-health-domain-security
source_filename: koda-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts (0-working/probe-domain-security.py, plus manual\n  probes of the application, API, and patient-facing hosts the script does not reach because Koda\n  publishes no OpenAPI servers[])\nhosts:\n- host: www.kodahealthcare.com\n  role: marketing site\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 11:05:05 2026 GMT\n  hsts: false\n- host: app.kodahealthcare.com\n  role: patient/provider application (S3 + CloudFront)\n  https: true\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  notes: >-\n    Strongest posture of the estate — also sets CSP with report-uri, X-Frame-Options DENY,\n    X-Content-Type-Options nosniff, Cross-Origin-Opener-Policy same-origin, Referrer-Policy no-referrer,\n    and Permissions-Policy denying geolocation/microphone/camera.\n- host: api.kodahealthcare.com\n  role: closed backend API\
  \ (AWS ELB, awselb/2.0); 403 to all unauthenticated requests\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 20 23:59:59 2026 GMT\n  hsts: false\n- host: koda.health\n  role: patient-facing marketing site\n  https: true\n  cert_expires: Sep 24 01:04:29 2026 GMT\n  hsts: false\ndomains:\n- domain: kodahealthcare.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: koda.health\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n  dmarc_policy: null\nfindings:\n- HSTS is enabled only on app.kodahealthcare.com; the marketing, patient, and API hosts do not set it.\n- DMARC on kodahealthcare.com is published at p=none (monitor only), not quarantine or reject.\n- koda.health publishes no SPF, no DMARC, and no CAA, though DNSSEC is signed.\n- api.kodahealthcare.com negotiates TLS 1.2 where the marketing host reaches TLS 1.3.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/koda-health/refs/heads/main/security/koda-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Health Care
- Digital Health
- Advance Care Planning
- Serious Illness Care
- Chronic Kidney Disease
- Patient Engagement
- Clinical Decision Support
- EMR Integration
- HL7 FHIR
- Interoperability
- HIPAA
- Value Based Care
---
