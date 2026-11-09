---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: benawf.com
  spf: true
hosts:
- cert_expires: Dec  4 23:04:10 2026 GMT
  host: benawf.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Benawf Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BenAwf, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BenAwf
provider_slug: benawf-com
slug: benawf-com-domain-security
source_filename: benawf-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: benawf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:04:10 2026 GMT\n  hsts: false\ndomains:\n- domain: benawf.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/benawf-com/security/benawf-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Trading
- Finance
- Platform
- Strategy
- Backtesting
---
