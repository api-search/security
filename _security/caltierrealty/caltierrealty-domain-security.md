---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: caltier.fund
  spf: true
hosts:
- cert_expires: Dec 30 05:01:40 2026 GMT
  host: www.caltier.fund
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Caltierrealty Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Caltierrealty, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Caltierrealty
provider_slug: caltierrealty
slug: caltierrealty-domain-security
source_filename: caltierrealty-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.caltier.fund\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 05:01:40 2026 GMT\n  hsts: false\ndomains:\n- domain: caltier.fund\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caltierrealty/refs/heads/main/security/caltierrealty-domain-security.yml
summary_line: TLSv1.3
tags:
- Real Estate
- Crowdfunding
- Investment
- Multi-family
- FinTech
---
