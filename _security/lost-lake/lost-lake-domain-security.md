---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: lostlakegames.com
  spf: false
hosts:
- cert_expires: Jan 16 23:59:59 2027 GMT
  host: lostlakegames.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lost Lake Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lost Lake Games, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Lost Lake Games
provider_slug: lost-lake
slug: lost-lake-domain-security
source_filename: lost-lake-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lostlakegames.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: lostlakegames.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lost-lake/refs/heads/main/security/lost-lake-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Video Games
- Gaming
- Game Studio
- Entertainment
- Seattle
- Consumer
---
