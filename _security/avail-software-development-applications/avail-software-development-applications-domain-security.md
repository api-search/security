---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getavail.com
  spf: true
hosts:
- cert_expires: Nov 17 19:34:40 2026 GMT
  host: www.getavail.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Avail Software Development Applications Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Avail Software Development Applications, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Avail Software Development Applications
provider_slug: avail-software-development-applications
slug: avail-software-development-applications-domain-security
source_filename: avail-software-development-applications-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getavail.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 19:34:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getavail.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avail-software-development-applications/refs/heads/main/security/avail-software-development-applications-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Content Management
- AEC
- Revit
- AutoCAD
- Civil 3D
- BIM
---
