---
description: ''
domains:
- caa:
  - 8ux6i6z1.up.railway.app.
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: faxivo.com
  spf: false
hosts:
- cert_expires: Jan  4 02:29:40 2027 GMT
  host: www.faxivo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Faxivo Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Faxivo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: Faxivo
provider_slug: faxivo-com
slug: faxivo-com-domain-security
source_filename: faxivo-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.faxivo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 02:29:40 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: faxivo.com\n  dnssec: true\n  caa:\n  - 8ux6i6z1.up.railway.app.\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/faxivo-com/security/faxivo-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- AI
- AgenticInternet
- Services
- Communication
---
