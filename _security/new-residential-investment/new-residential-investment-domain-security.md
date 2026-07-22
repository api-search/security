---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rithmcap.com
  spf: true
hosts:
- cert_expires: Aug 31 23:59:59 2026 GMT
  host: www.rithmcap.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: New Residential Investment Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for New Residential Investment Corp (Rithm Capital), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: New Residential Investment Corp (Rithm Capital)
provider_slug: new-residential-investment
slug: new-residential-investment-domain-security
source_filename: new-residential-investment-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rithmcap.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: rithmcap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/new-residential-investment/refs/heads/main/security/new-residential-investment-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Mortgage REIT
- Real Estate Investment Trust
- Asset Management
- Mortgage Origination
- Mortgage Servicing
- Alternative Investments
- Hedge Funds
- Private Credit
- Commercial Real Estate
- Single-Family Rental
- Financial Services
- Fortune 1000
---
