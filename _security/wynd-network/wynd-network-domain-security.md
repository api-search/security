---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wyndlabs.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: grass.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getgrass.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wynd.network
  spf: true
hosts:
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: wyndlabs.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 23:59:59 2026 GMT
  host: www.grass.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 16:28:57 2026 GMT
  host: app.grass.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 10:46:18 2026 GMT
  host: wynd.network
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 13:03:29 2026 GMT
  host: api.getgrass.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wynd Network Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wynd Network, probed live across 5 host(s) and 4 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Wynd Network
provider_slug: wynd-network
slug: wynd-network-domain-security
source_filename: wynd-network-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wyndlabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: false\n- host: www.grass.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 23:59:59 2026 GMT\n  hsts: false\n- host: app.grass.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 16:28:57 2026 GMT\n  hsts: false\n- host: wynd.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 10:46:18 2026 GMT\n  hsts: false\n- host: api.getgrass.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 13:03:29 2026 GMT\n  hsts: false\ndomains:\n- domain: wyndlabs.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: grass.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: getgrass.io\n  dnssec: false\n  caa: []\n  spf: true\n\
  \  dmarc: true\n  dmarc_policy: quarantine\n- domain: wynd.network\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wynd-network/refs/heads/main/security/wynd-network-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Depin
- Bandwidth
- Web Scraping
- AI Training Data
- Cryptocurrency
- Solana
---
