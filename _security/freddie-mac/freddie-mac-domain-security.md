---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: freddiemac.com
  spf: true
hosts:
- cert_expires: Sep  1 23:59:59 2026 GMT
  host: www.freddiemac.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 23:59:59 2026 GMT
  host: sf.freddiemac.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Freddie Mac Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Freddie Mac, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Freddie Mac
provider_slug: freddie-mac
slug: freddie-mac-domain-security
source_filename: freddie-mac-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.freddiemac.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sf.freddiemac.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: freddiemac.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freddie-mac/refs/heads/main/security/freddie-mac-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal-Government
- Housing
- Mortgage
- Lending
- Servicing
- Fortune 100
---
