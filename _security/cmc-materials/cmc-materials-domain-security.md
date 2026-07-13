---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cmcmaterials.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: entegris.com
  spf: true
hosts:
- host: www.cmcmaterials.com
  https: false
- cert_expires: Oct  6 23:59:59 2026 GMT
  host: www.entegris.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cmc Materials Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CMC Materials, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CMC Materials
provider_slug: cmc-materials
slug: cmc-materials-domain-security
source_filename: cmc-materials-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cmcmaterials.com\n  https: false\n- host: www.entegris.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cmcmaterials.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: entegris.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cmc-materials/refs/heads/main/security/cmc-materials-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Semiconductors
- Materials
- Manufacturing
- CMP
- Specialty Chemicals
---
