---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: noctuasky.com
  spf: true
hosts:
- cert_expires: Sep 23 17:37:46 2026 GMT
  host: api.noctuasky.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Noctua Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Noctua, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Noctua
provider_slug: noctua
slug: noctua-domain-security
source_filename: noctua-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.noctuasky.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 23 17:37:46 2026 GMT\n  hsts: null\ndomains:\n- domain: noctuasky.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/noctua/refs/heads/main/security/noctua-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Science And Math
- Public APIs
---
