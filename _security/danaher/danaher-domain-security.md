---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: danaher.com
  spf: true
hosts:
- cert_expires: Dec 29 23:59:59 2026 GMT
  host: www.danaher.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Danaher Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Danaher, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Danaher
provider_slug: danaher
slug: danaher-domain-security
source_filename: danaher-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.danaher.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: danaher.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/danaher/refs/heads/main/security/danaher-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Biotechnology
- Conglomerate
- Diagnostics
- Life Sciences
- Medical Devices
- Fortune 500
---
