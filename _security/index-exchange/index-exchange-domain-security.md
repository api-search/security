---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: indexexchange.com
  spf: true
hosts:
- cert_expires: Jan 11 21:02:47 2027 GMT
  host: www.indexexchange.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Index Exchange Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Index Exchange, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Index Exchange
provider_slug: index-exchange
slug: index-exchange-domain-security
source_filename: index-exchange-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.indexexchange.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 21:02:47 2027 GMT\n  hsts: false\ndomains:\n- domain: indexexchange.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/index-exchange/refs/heads/main/security/index-exchange-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Advertising
- Programmatic
- Supply Side Platform
- Real-time Bidding
- Media Technology
- Company
---
