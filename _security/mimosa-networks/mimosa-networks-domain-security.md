---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: mimosa.co
  spf: true
hosts:
- cert_expires: Dec 12 16:32:36 2026 GMT
  host: mimosa.co
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mimosa Networks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mimosa Networks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Mimosa Networks
provider_slug: mimosa-networks
slug: mimosa-networks-domain-security
source_filename: mimosa-networks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mimosa.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 16:32:36 2026 GMT\n  hsts: false\ndomains:\n- domain: mimosa.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/mimosa-networks/security/mimosa-networks-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Fixed Wireless
- Connectivity
- Networking
- Infrastructure
---
