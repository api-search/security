---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: joinhonor.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: honorcare.com
  spf: true
hosts:
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: www.joinhonor.com
  hsts: true
  hsts_max_age: 5184000
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 26 04:14:28 2026 GMT
  host: www.honorcare.com
  hsts: true
  hsts_max_age: 5184000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Honor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Honor, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Honor
provider_slug: honor
slug: honor-domain-security
source_filename: honor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.joinhonor.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 5184000\n- host: www.honorcare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 04:14:28 2026 GMT\n  hsts: true\n  hsts_max_age: 5184000\ndomains:\n- domain: joinhonor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: honorcare.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/honor/refs/heads/main/security/honor-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Home Care
- Senior Care
- Aging
- Health Tech
- Care Platform
- Caregivers
- Home Instead
- No Public API
---
