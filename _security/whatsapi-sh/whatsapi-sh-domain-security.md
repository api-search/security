---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: whatsapi.sh
  spf: true
hosts:
- cert_expires: Jan 19 20:53:00 2027 GMT
  host: whatsapi.sh
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: whatsapi-sh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for whatsapi-sh, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: whatsapi-sh
provider_slug: whatsapi-sh
slug: whatsapi-sh-domain-security
source_filename: whatsapi-sh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: whatsapi.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 20:53:00 2027 GMT\n  hsts: false\ndomains:\n- domain: whatsapi.sh\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/whatsapi-sh/security/whatsapi-sh-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Messaging
- WhatsApp
- Developer Tools
---
