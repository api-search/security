---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: berkshirehathaway.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bnsf.com
  spf: true
hosts:
- cert_expires: Aug 11 23:53:04 2026 GMT
  host: www.berkshirehathaway.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 19:46:14 2026 GMT
  host: www.bnsf.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Berkshire Hathaway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Berkshire Hathaway, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Berkshire Hathaway
provider_slug: berkshire-hathaway
slug: berkshire-hathaway-domain-security
source_filename: berkshire-hathaway-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.berkshirehathaway.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 23:53:04 2026 GMT\n  hsts: false\n- host: www.bnsf.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 14 19:46:14 2026 GMT\n  hsts: false\ndomains:\n- domain: berkshirehathaway.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: bnsf.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/berkshire-hathaway/refs/heads/main/security/berkshire-hathaway-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Conglomerate
- Energy
- Finance
- Freight Rail
- Insurance
- Investment
- Manufacturing
- Retail
- Utilities
- Fortune 100
---
