---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cellbox-solutions.com
  spf: true
hosts:
- cert_expires: Nov 29 23:59:59 2026 GMT
  host: cellbox-solutions.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cellboxsolutions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cellboxsolutions, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cellboxsolutions
provider_slug: cellboxsolutions
slug: cellboxsolutions-domain-security
source_filename: cellboxsolutions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cellbox-solutions.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: cellbox-solutions.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cellboxsolutions/refs/heads/main/security/cellboxsolutions-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Bio-Medical
- Logistics
- Cell Transport
- CO2 Incubator
- Life Sciences
---
