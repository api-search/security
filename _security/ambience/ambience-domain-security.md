---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: ambiencehealthcare.com
  spf: true
hosts:
- cert_expires: Aug 22 21:49:39 2026 GMT
  host: www.ambiencehealthcare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 16:57:22 2026 GMT
  host: docs.ambiencehealthcare.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ambience Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ambience, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Ambience
provider_slug: ambience
slug: ambience-domain-security
source_filename: ambience-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ambiencehealthcare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 21:49:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.ambiencehealthcare.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 10 16:57:22 2026 GMT\n  hsts: false\ndomains:\n- domain: ambiencehealthcare.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ambience/refs/heads/main/security/ambience-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Artificial Intelligence
- Clinical Documentation
- Ambient AI
- Medical Coding
- EHR Integration
- Health IT
---
