---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: provivi.com
  spf: true
hosts:
- cert_expires: Sep 19 23:59:59 2026 GMT
  host: www.provivi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:06:52 2026 GMT
  host: api.provivi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Provivi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Provivi, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Provivi
provider_slug: provivi
slug: provivi-domain-security
source_filename: provivi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.provivi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:59:59 2026 GMT\n  hsts: false\n- host: api.provivi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:06:52 2026 GMT\n  hsts: false\ndomains:\n- domain: provivi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/provivi/refs/heads/main/security/provivi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Agriculture
- AgTech
- Biotechnology
- Crop Protection
- Pheromones
- Sustainability
- Content Management
- GraphQL
---
