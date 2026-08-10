---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: villagemd.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: villagemedical.com
  spf: true
hosts:
- cert_expires: Sep 18 15:30:15 2026 GMT
  host: www.villagemd.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 03:29:45 2026 GMT
  host: www.villagemedical.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Villagemd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VillageMD, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: VillageMD
provider_slug: villagemd
slug: villagemd-domain-security
source_filename: villagemd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.villagemd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 15:30:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.villagemedical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 03:29:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: villagemd.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: villagemedical.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\nx-note: >-\n  www.villagemedical.com is the patient-facing brand host and was probed by hand with\n  the same dig/openssl/HEAD checks the script runs; it is not reachable from a Website\n  or Portal pointer in apis.yml, so probe-domain-security.py did not pick it up.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/villagemd/refs/heads/main/security/villagemd-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Primary Care
- Value-Based Care
- Medical Practices
- Urgent Care
- Telehealth
- Patient Care
- Clinics
---
