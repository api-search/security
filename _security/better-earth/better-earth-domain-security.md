---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: betterearth.org
  spf: false
hosts:
- cert_expires: Oct 29 02:03:31 2026 GMT
  host: betterearth.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Better Earth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Better Earth, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Better Earth
provider_slug: better-earth
slug: better-earth-domain-security
source_filename: better-earth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: betterearth.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 02:03:31 2026 GMT\n  hsts: false\ndomains:\n- domain: betterearth.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/better-earth/refs/heads/main/security/better-earth-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Climate
- Philanthropy
- Events
- Sustainability
- Community
---
