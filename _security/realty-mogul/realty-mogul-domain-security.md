---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: realtymogul.com
  spf: true
hosts:
- cert_expires: Aug 16 17:52:20 2026 GMT
  host: realtymogul.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Realty Mogul Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Realty Mogul, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Realty Mogul
provider_slug: realty-mogul
slug: realty-mogul-domain-security
source_filename: realty-mogul-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: realtymogul.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 17:52:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: realtymogul.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/realty-mogul/refs/heads/main/security/realty-mogul-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Real Estate
- Crowdfunding
- Investing
- REIT
- Commercial Real Estate
- FinTech
---
