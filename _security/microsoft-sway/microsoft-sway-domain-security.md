---
description: ''
domains:
- caa:
  - 0 iodef "mailto:caarecordaware@microsoft.com"
  - 0 issue "microsoft.com"
  - 0 issue "digicert.com"
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cloud.microsoft
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
hosts:
- cert_expires: Oct 30 09:53:29 2026 GMT
  host: sway.cloud.microsoft
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 17 19:55:21 2027 GMT
  host: www.microsoft.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 20 00:51:37 2026 GMT
  host: support.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Microsoft Sway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Sway, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Sway
provider_slug: microsoft-sway
slug: microsoft-sway-domain-security
source_filename: microsoft-sway-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sway.cloud.microsoft\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 30 09:53:29 2026 GMT\n  hsts: null\n- host: www.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 19:55:21 2027 GMT\n  hsts: false\n- host: support.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 00:51:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cloud.microsoft\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:caarecordaware@microsoft.com\"\n  - 0 issue \"microsoft.com\"\n  - 0 issue \"digicert.com\"\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-sway/refs/heads/main/security/microsoft-sway-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Content Creation
- Microsoft
- Microsoft 365
- Presentations
- Storytelling
---
