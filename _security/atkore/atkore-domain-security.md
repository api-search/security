---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: atkore.com
  spf: true
hosts:
- cert_expires: Sep 18 02:14:28 2026 GMT
  host: www.atkore.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Atkore Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atkore, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Atkore
provider_slug: atkore
slug: atkore-domain-security
source_filename: atkore-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.atkore.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 02:14:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: atkore.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atkore/refs/heads/main/security/atkore-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- BIM
- Cable Management
- Conduit
- Construction
- Electrical
- Manufacturing
- Raceway
---
