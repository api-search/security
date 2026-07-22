---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: zim.com
  spf: true
hosts:
- cert_expires: Sep  1 23:59:59 2026 GMT
  host: www.zim.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zim Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ZIM Integrated Shipping Services, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ZIM Integrated Shipping Services
provider_slug: zim-com
slug: zim-com-domain-security
source_filename: zim-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zim.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: zim.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zim-com/refs/heads/main/security/zim-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Shipping
- Container Shipping
- Ocean Freight
- Logistics
- Supply Chain
- Maritime
- Container Tracking
- EDI
- Electronic Bill of Lading
- Cargo Visibility
- Israel
- Transportation
---
