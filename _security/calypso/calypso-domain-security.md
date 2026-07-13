---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nasdaq.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: calypso.com
  spf: true
hosts:
- cert_expires: Sep 26 23:59:59 2026 GMT
  host: www.nasdaq.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: www.calypso.com
  https: false
kind: domain-security
layout: security
method: probed
name: Calypso Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Calypso, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Calypso
provider_slug: calypso
slug: calypso-domain-security
source_filename: calypso-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nasdaq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  hsts: false\n- host: www.calypso.com\n  https: false\ndomains:\n- domain: nasdaq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: calypso.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/calypso/refs/heads/main/security/calypso-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Capital Markets
- Collateral Management
- Enterprise Software
- Financial Technology
- Post-Trade Processing
- Risk Management
- Trading
- Treasury
---
