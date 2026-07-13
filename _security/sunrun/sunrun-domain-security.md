---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sunrun.com
  spf: true
hosts:
- cert_expires: Oct 12 23:59:59 2026 GMT
  host: www.sunrun.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: developer.sunrun.com
  https: false
- host: api.sunrun.com
  https: false
kind: domain-security
layout: security
method: probed
name: Sunrun Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sunrun, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sunrun
provider_slug: sunrun
slug: sunrun-domain-security
source_filename: sunrun-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sunrun.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 23:59:59 2026 GMT\n  hsts: false\n- host: developer.sunrun.com\n  https: false\n- host: api.sunrun.com\n  https: false\ndomains:\n- domain: sunrun.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sunrun/refs/heads/main/security/sunrun-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Residential Solar
- Clean Energy
---
