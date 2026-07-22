---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: onsitedental.com
  spf: true
hosts:
- cert_expires: Aug 29 18:48:44 2026 GMT
  host: onsitedental.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Onsitedental Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Onsitedental, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Onsitedental
provider_slug: onsitedental
slug: onsitedental-domain-security
source_filename: onsitedental-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: onsitedental.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 18:48:44 2026 GMT\n  hsts: false\ndomains:\n- domain: onsitedental.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onsitedental/refs/heads/main/security/onsitedental-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Dental
- Healthcare
- Employee Benefits
- Corporate Wellness
- Oral Health
- Mobile Health
- Workplace Health
---
