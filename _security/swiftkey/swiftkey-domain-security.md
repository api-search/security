---
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:caarecordaware@microsoft.com"
  - 0 contactemail "caarecordaware@microsoft.com"
  - 0 issue "microsoft.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: swiftkey.com
  spf: true
hosts:
- cert_expires: Nov 26 07:38:57 2026 GMT
  host: www.swiftkey.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Swiftkey Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Swiftkey, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Swiftkey
provider_slug: swiftkey
slug: swiftkey-domain-security
source_filename: swiftkey-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.swiftkey.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 07:38:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: swiftkey.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:caarecordaware@microsoft.com\"\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  - 0 issue \"microsoft.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swiftkey/refs/heads/main/security/swiftkey-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Keyboard
- Predictive Text
- Machine Learning
- Mobile
- Microsoft
---
