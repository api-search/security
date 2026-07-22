---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: saul.com
  spf: true
hosts:
- cert_expires: Sep 18 17:08:46 2026 GMT
  host: www.saul.com
  hsts: true
  hsts_max_age: 1000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Saul Ewing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Saul Ewing LLP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Saul Ewing LLP
provider_slug: saul-ewing
slug: saul-ewing-domain-security
source_filename: saul-ewing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.saul.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 17:08:46 2026 GMT\n  hsts: true\n  hsts_max_age: 1000\ndomains:\n- domain: saul.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/saul-ewing/refs/heads/main/security/saul-ewing-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Legal
- Law Firm
- Litigation
- Corporate
- Mergers And Acquisitions
- Bankruptcy
- Real Estate
- Public Finance
- Life Sciences
- Intellectual Property
---
