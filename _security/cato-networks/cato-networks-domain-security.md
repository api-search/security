---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: catonetworks.com
  spf: true
hosts:
- cert_expires: Mar 12 13:23:30 2027 GMT
  host: www.catonetworks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 13:06:45 2026 GMT
  host: api.catonetworks.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cato Networks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cato Networks, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cato Networks
provider_slug: cato-networks
slug: cato-networks-domain-security
source_filename: cato-networks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.catonetworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 12 13:23:30 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.catonetworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 13:06:45 2026 GMT\n  hsts: null\ndomains:\n- domain: catonetworks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cato-networks/refs/heads/main/security/cato-networks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cybersecurity
- SASE
- SSE
- Networking
- Security
- SD-WAN
- Zero Trust
- GraphQL
- API
---
