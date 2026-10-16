---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: changba.com
  spf: true
hosts:
- cert_expires: Oct 19 23:59:59 2026 GMT
  host: changba.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Changba Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Changba, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Changba
provider_slug: changba
slug: changba-domain-security
source_filename: changba-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: changba.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 19 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: changba.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/changba/refs/heads/main/security/changba-domain-security.yml
summary_line: TLSv1.2
tags:
- Music
- Karaoke
- MobileApp
- Community
- Entertainment
---
