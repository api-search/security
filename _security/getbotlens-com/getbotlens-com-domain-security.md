---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: getbotlens.com
  spf: false
hosts:
- cert_expires: Jan  8 00:25:32 2027 GMT
  host: getbotlens.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Getbotlens Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for getbotlens-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: getbotlens-com
provider_slug: getbotlens-com
slug: getbotlens-com-domain-security
source_filename: getbotlens-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getbotlens.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 00:25:32 2027 GMT\n  hsts: false\ndomains:\n- domain: getbotlens.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/getbotlens-com/security/getbotlens-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Bot Detection
- Analytics
- Security
- AI
- Web
---
