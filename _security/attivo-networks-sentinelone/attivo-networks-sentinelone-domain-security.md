---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: attivonetworks.com
  spf: true
hosts:
- cert_expires: Sep  1 17:55:56 2026 GMT
  host: www.attivonetworks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Attivo Networks Sentinelone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Attivo Networks (SentinelOne), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Attivo Networks (SentinelOne)
provider_slug: attivo-networks-sentinelone
slug: attivo-networks-sentinelone-domain-security
source_filename: attivo-networks-sentinelone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.attivonetworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 17:55:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: attivonetworks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/attivo-networks-sentinelone/refs/heads/main/security/attivo-networks-sentinelone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Cybersecurity
- Identity
- ITDR
- Endpoint Security
- Deception
- XDR
---
