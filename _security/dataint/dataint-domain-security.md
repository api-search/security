---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dataint.mx
  spf: true
hosts:
- cert_expires: Aug 25 08:00:19 2026 GMT
  host: dataint.mx
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dataint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DataInt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DataInt
provider_slug: dataint
slug: dataint-domain-security
source_filename: dataint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dataint.mx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 08:00:19 2026 GMT\n  hsts: null\ndomains:\n- domain: dataint.mx\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dataint/refs/heads/main/security/dataint-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
