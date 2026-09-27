---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: repligen.com
  spf: true
hosts:
- cert_expires: Nov  4 20:06:41 2026 GMT
  host: www.repligen.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Avitide Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Avitide, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Avitide
provider_slug: avitide
slug: avitide-domain-security
source_filename: avitide-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.repligen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 20:06:41 2026 GMT\n  hsts: false\ndomains:\n- domain: repligen.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avitide/refs/heads/main/security/avitide-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Bioprocessing
- DownstreamProcessing
- Chromatography
- Filtration
- Biopharma
---
