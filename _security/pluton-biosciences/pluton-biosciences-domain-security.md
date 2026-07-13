---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: plutonbio.com
  spf: true
hosts:
- cert_expires: Aug 29 08:40:42 2026 GMT
  host: www.plutonbio.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pluton Biosciences Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pluton Biosciences, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Pluton Biosciences
provider_slug: pluton-biosciences
slug: pluton-biosciences-domain-security
source_filename: pluton-biosciences-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.plutonbio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 08:40:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: plutonbio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pluton-biosciences/refs/heads/main/security/pluton-biosciences-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agriculture
- AgTech
- Biotech
- Microbials
- Soil Carbon
- Discovery Platform
---
