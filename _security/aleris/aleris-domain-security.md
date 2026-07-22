---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aleris.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: novelis.com
  spf: true
hosts:
- host: www.aleris.com
  https: false
- cert_expires: Sep 18 01:13:45 2026 GMT
  host: novelis.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aleris Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for aleris, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: aleris
provider_slug: aleris
slug: aleris-domain-security
source_filename: aleris-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aleris.com\n  https: false\n- host: novelis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 01:13:45 2026 GMT\n  hsts: false\ndomains:\n- domain: aleris.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: novelis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aleris/refs/heads/main/security/aleris-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Aluminum
- Manufacturing
- Aerospace
- Automotive
- Industrial
- Materials
---
