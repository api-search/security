---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: foxcorporation.com
  spf: true
hosts:
- cert_expires: Sep  5 23:59:59 2026 GMT
  host: www.foxcorporation.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Twenty First Century Fox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Twenty-First Century Fox, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Twenty-First Century Fox
provider_slug: twenty-first-century-fox
slug: twenty-first-century-fox-domain-security
source_filename: twenty-first-century-fox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.foxcorporation.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: foxcorporation.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/twenty-first-century-fox/refs/heads/main/security/twenty-first-century-fox-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Media
- Entertainment
- Film
- Television
- Broadcasting
- Fortune 100
---
