---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aquis.eu
  spf: true
hosts:
- cert_expires: Dec 23 12:28:36 2026 GMT
  host: www.aquis.eu
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aquis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AQUIS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AQUIS
provider_slug: aquis
slug: aquis-domain-security
source_filename: aquis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aquis.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 12:28:36 2026 GMT\n  hsts: null\ndomains:\n- domain: aquis.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aquis/refs/heads/main/security/aquis-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Finance
- Exchange
- Market Data
- Trading
---
