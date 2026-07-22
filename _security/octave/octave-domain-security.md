---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: findoctave.com
  spf: true
hosts:
- cert_expires: Sep  1 19:45:58 2026 GMT
  host: findoctave.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Octave Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Octave, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Octave
provider_slug: octave
slug: octave-domain-security
source_filename: octave-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: findoctave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 19:45:58 2026 GMT\n  hsts: false\ndomains:\n- domain: findoctave.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/octave/refs/heads/main/security/octave-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Health
- Mental Health
- Therapy
- Healthcare
- Telehealth
- Behavioral Health
- Wellness
---
