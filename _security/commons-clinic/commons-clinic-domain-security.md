---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: commonsclinic.com
  spf: true
hosts:
- cert_expires: Oct 23 07:24:24 2026 GMT
  host: commonsclinic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Commons Clinic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Commons Clinic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Commons Clinic
provider_slug: commons-clinic
slug: commons-clinic-domain-security
source_filename: commons-clinic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: commonsclinic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 07:24:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: commonsclinic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commons-clinic/refs/heads/main/security/commons-clinic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Orthopedics
- Spine
- Sports Medicine
- Musculoskeletal
- Physical Therapy
- Surgery
- Pain Management
- Preventive Health
- Clinics
---
