---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bigleaf.net
  spf: true
hosts:
- cert_expires: Nov 24 02:58:40 2026 GMT
  host: www.bigleaf.net
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bigleaf Networks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bigleaf Networks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bigleaf Networks
provider_slug: bigleaf-networks
slug: bigleaf-networks-domain-security
source_filename: bigleaf-networks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bigleaf.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 02:58:40 2026 GMT\n  hsts: false\ndomains:\n- domain: bigleaf.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bigleaf-networks/refs/heads/main/security/bigleaf-networks-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Cloud-Managed WAN
- Network Optimization
- Hybrid WAN
- 5G Integration
- Enterprise Connectivity
- Company
---
