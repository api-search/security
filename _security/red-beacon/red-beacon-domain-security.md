---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: redbeacon.com
  spf: true
hosts:
- cert_expires: Oct 18 03:00:56 2026 GMT
  host: www.redbeacon.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Red Beacon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Red Beacon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Red Beacon
provider_slug: red-beacon
slug: red-beacon-domain-security
source_filename: red-beacon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.redbeacon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 03:00:56 2026 GMT\n  hsts: null\ndomains:\n- domain: redbeacon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/red-beacon/refs/heads/main/security/red-beacon-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Home Services
- Marketplace
- Local Services
- Consumer
- Acquired
- Defunct
---
