---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: denso.com
  spf: true
hosts:
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: www.denso.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Denso Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Denso, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Denso
provider_slug: denso
slug: denso-domain-security
source_filename: denso-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.denso.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: denso.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/denso/refs/heads/main/security/denso-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Automotive
- Tier 1 Supplier
- Components
- Thermal Management
- Electrification
---
