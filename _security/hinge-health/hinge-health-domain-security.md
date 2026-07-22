---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hingehealth.com
  spf: true
hosts:
- cert_expires: Sep 25 07:30:18 2026 GMT
  host: www.hingehealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hinge Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hinge Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hinge Health
provider_slug: hinge-health
slug: hinge-health-domain-security
source_filename: hinge-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hingehealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 07:30:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hingehealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hinge-health/refs/heads/main/security/hinge-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Digital Health
- Musculoskeletal Care
- MSK
- Virtual Physical Therapy
- Pelvic Health
- Chronic Pain
- Digital Therapeutics
- Wearables
- Enso
- HingeConnect
- EMR Interoperability
- Health Plans
- Employer Health
- Value Based Care
- Public Company
---
