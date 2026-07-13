---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: lass-net.org
  spf: false
hosts:
- cert_expires: Sep  9 18:59:40 2026 GMT
  host: pm25.lass-net.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pm2 5 Open Data Portal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PM2.5 Open Data Portal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: PM2.5 Open Data Portal
provider_slug: pm2-5-open-data-portal
slug: pm2-5-open-data-portal-domain-security
source_filename: pm2-5-open-data-portal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pm25.lass-net.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 18:59:40 2026 GMT\n  hsts: false\ndomains:\n- domain: lass-net.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pm2-5-open-data-portal/refs/heads/main/security/pm2-5-open-data-portal-domain-security.yml
summary_line: TLSv1.3
tags:
- Environment
- Public APIs
---
