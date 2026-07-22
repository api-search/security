---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pluribusnetworks.com
  spf: true
hosts:
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: pluribusnetworks.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pluribus Networks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pluribus Networks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Pluribus Networks
provider_slug: pluribus-networks
slug: pluribus-networks-domain-security
source_filename: pluribus-networks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pluribusnetworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: pluribusnetworks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pluribus-networks/refs/heads/main/security/pluribus-networks-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Networking
- Software-Defined Networking
- Open Networking
- Data Center
- Network Operating System
- Acquired
---
