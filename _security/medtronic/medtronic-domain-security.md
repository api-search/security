---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: medtronic.com
  spf: true
hosts:
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: www.medtronic.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: developer.medtronic.com
  https: false
- host: api.medtronic.com
  https: false
kind: domain-security
layout: security
method: probed
name: Medtronic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Medtronic, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Medtronic
provider_slug: medtronic
slug: medtronic-domain-security
source_filename: medtronic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.medtronic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: false\n- host: developer.medtronic.com\n  https: false\n- host: api.medtronic.com\n  https: false\ndomains:\n- domain: medtronic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medtronic/refs/heads/main/security/medtronic-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Healthcare
- Medical Devices
---
