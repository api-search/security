---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lakesidesoftware.com
  spf: true
hosts:
- cert_expires: Sep 14 16:59:27 2026 GMT
  host: www.lakesidesoftware.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 17:17:37 2026 GMT
  host: documentation.lakesidesoftware.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: cloud.lakesidesoftware.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lakeside Software Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lakeside Software, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lakeside Software
provider_slug: lakeside-software
slug: lakeside-software-domain-security
source_filename: lakeside-software-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lakesidesoftware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 16:59:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: documentation.lakesidesoftware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 17:17:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cloud.lakesidesoftware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lakesidesoftware.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lakeside-software/refs/heads/main/security/lakeside-software-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Digital Employee Experience
- Endpoint Monitoring
- IT Operations
- Observability
- Device Management
- End User Computing
- Analytics
- Virtual Desktop
- ITSM
---
