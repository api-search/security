---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: txone.com
  spf: true
hosts:
- cert_expires: Mar  8 23:59:59 2027 GMT
  host: www.txone.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Txone Networks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TXOne Networks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TXOne Networks
provider_slug: txone-networks
slug: txone-networks-domain-security
source_filename: txone-networks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.txone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: txone.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/txone-networks/refs/heads/main/security/txone-networks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Cybersecurity
- Operational Technology
- Industrial Control Systems
- Critical Infrastructure
- Endpoint Protection
- Network Security
- Vulnerability Management
- Manufacturing
---
