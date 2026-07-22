---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: elwyn.org
  spf: true
hosts:
- cert_expires: Oct  4 14:40:28 2026 GMT
  host: www.elwyn.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Elwyn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Elwyn, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Elwyn
provider_slug: elwyn
slug: elwyn-domain-security
source_filename: elwyn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.elwyn.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 14:40:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: elwyn.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elwyn/refs/heads/main/security/elwyn-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Nonprofit
- Human Services
- Disability Services
- Behavioral Health
- Intellectual Disabilities
- Developmental Disabilities
- Autism Services
- Early Intervention
- Education
- Crisis Services
- Pennsylvania
---
