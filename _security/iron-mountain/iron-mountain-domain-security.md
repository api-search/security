---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "www.digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ironmountain.com
  spf: true
hosts:
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: www.ironmountain.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Iron Mountain Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Iron Mountain, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Iron Mountain
provider_slug: iron-mountain
slug: iron-mountain-domain-security
source_filename: iron-mountain-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ironmountain.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: ironmountain.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"www.digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iron-mountain/refs/heads/main/security/iron-mountain-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Records Management
- Information Management
- Data Centers
- Digital Transformation
- Storage
- Fortune 1000
---
