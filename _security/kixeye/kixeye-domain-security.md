---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kixeye.com
  spf: true
hosts:
- cert_expires: Jan 30 23:59:59 2027 GMT
  host: www.kixeye.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 30 23:59:59 2027 GMT
  host: api.kixeye.com
  hsts: false
  https: true
  note: private game-services backend; serves /.well-known/openid-configuration and /.well-known/jwks, 404 at root
  tls_version: TLSv1.2
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: corp.kixeye.com
  hsts: false
  https: true
  server: AmazonS3
kind: domain-security
layout: security
method: probed
name: Kixeye Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kixeye, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kixeye
provider_slug: kixeye
slug: kixeye-domain-security
source_filename: kixeye-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kixeye.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  hsts: false\n- host: api.kixeye.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  hsts: false\n  note: private game-services backend; serves /.well-known/openid-configuration and /.well-known/jwks,\n    404 at root\n- host: corp.kixeye.com\n  https: true\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: false\n  server: AmazonS3\ndomains:\n- domain: kixeye.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kixeye/refs/heads/main/security/kixeye-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Gaming
- Video Games
- Game Development
- Mobile Games
- Strategy Games
- Free To Play
- Live Service
---
