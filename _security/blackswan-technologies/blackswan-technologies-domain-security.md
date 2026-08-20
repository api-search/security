---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: blackswantechnologies.ai
  ns: []
  resolves: false
  soa: null
  spf: false
  status: lapsed
- caa: []
  dmarc: false
  dnssec: false
  domain: caios.io
  mx: []
  resolves: true
  spf: false
  status: active-behind-cloudflare
hosts:
- host: www.blackswantechnologies.ai
  https: false
  reachable: false
  reason: DNS resolution failure (no NS, SOA, A, MX or TXT records)
- cert_issuer: C=US, O=Let's Encrypt, CN=YE2
  cert_not_after: '2026-10-17T08:22:51Z'
  cert_subject: CN=caios.io
  cert_verify: ok
  host: caios.io
  hsts: false
  http_status: 403
  http_status_note: Cloudflare challenge on every path, including the site root
  https: true
  server: cloudflare
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blackswan Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BlackSwan Technologies, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: BlackSwan Technologies
provider_slug: blackswan-technologies
slug: blackswan-technologies-domain-security
source_filename: blackswan-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nnote: >-\n  probe-domain-security.py returned \"unreachable\" for this provider because the corporate\n  domain blackswantechnologies.ai no longer resolves in DNS. This file records the manual\n  probe of both the defunct corporate domain and caios.io, the surviving domain of BST\n  LABS (BlackSwan Technologies' software engineering unit). Absence of a record is valid\n  recorded data.\nhosts:\n- host: www.blackswantechnologies.ai\n  https: false\n  reachable: false\n  reason: DNS resolution failure (no NS, SOA, A, MX or TXT records)\n- host: caios.io\n  https: true\n  http_status: 403\n  http_status_note: Cloudflare challenge on every path, including the site root\n  tls_version: TLSv1.3\n  cert_subject: CN=caios.io\n  cert_issuer: \"C=US, O=Let's Encrypt, CN=YE2\"\n  cert_not_after: '2026-10-17T08:22:51Z'\n  cert_verify: ok\n  hsts: false\n  server: cloudflare\ndomains:\n- domain: blackswantechnologies.ai\n  resolves: false\n  ns:\
  \ []\n  soa: null\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  status: lapsed\n- domain: caios.io\n  resolves: true\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  mx: []\n  status: active-behind-cloudflare\nx-evidence:\n  fetched: '2026-08-02'\n  tooling: dig (NS/SOA/A/MX/TXT/CAA/_dmarc), openssl s_client, curl -I\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blackswan-technologies/refs/heads/main/security/blackswan-technologies-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Artificial Intelligence
- Data Fabric
- Knowledge Graphs
- Enterprise Software
- Financial Crime
- KYC
- Compliance
- Open-Source
- Acquired
---
