---
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  - 0 issue "digicert.com"
  - 0 issue "microsoft.com"
  - 0 iodef "mailto:caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: glintinc.com
  spf: true
hosts:
- cert_expires: Dec 31 11:07:34 2026 GMT
  host: www.glintinc.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Glint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Glint, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Glint
provider_slug: glint
slug: glint-domain-security
source_filename: glint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.glintinc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 11:07:34 2026 GMT\n  hsts: null\ndomains:\n- domain: glintinc.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"microsoft.com\"\n  - 0 iodef \"mailto:caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glint/refs/heads/main/security/glint-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Employee Engagement
- Employee Experience
- Organizational Health
- People Analytics
- Survey
- HR Tech
- Microsoft Viva
---
