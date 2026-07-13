---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: magicthegathering.io
  spf: false
hosts:
- cert_expires: Aug 31 06:51:46 2026 GMT
  host: magicthegathering.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Magic The Gathering Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Magic The Gathering, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Magic The Gathering
provider_slug: magic-the-gathering
slug: magic-the-gathering-domain-security
source_filename: magic-the-gathering-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: magicthegathering.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 06:51:46 2026 GMT\n  hsts: false\ndomains:\n- domain: magicthegathering.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/magic-the-gathering/refs/heads/main/security/magic-the-gathering-domain-security.yml
summary_line: TLSv1.3
tags:
- Games And Comics
- Public APIs
---
