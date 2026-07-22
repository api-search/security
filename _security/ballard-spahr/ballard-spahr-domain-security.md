---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ballardspahr.com
  spf: true
hosts:
- cert_expires: Mar 25 23:59:59 2027 GMT
  host: www.ballardspahr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ballard Spahr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ballard Spahr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ballard Spahr
provider_slug: ballard-spahr
slug: ballard-spahr-domain-security
source_filename: ballard-spahr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ballardspahr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 25 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ballardspahr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ballard-spahr/refs/heads/main/security/ballard-spahr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Banking
- Bankruptcy
- Class Action
- Commercial Litigation
- Consumer Financial Services
- Corporate
- CFPB
- Cybersecurity
- Data Privacy
- Employment Law
- Environmental
- ESG
- Finance
- Fintech
- Government Affairs
- Healthcare
- Intellectual Property
- Labor
- Law
- Law Firm
- Legal
- Legal Services
- Litigation
- Mergers and Acquisitions
- Mortgage
- Privacy
- Private Equity
- Public Finance
- Real Estate
- Real Estate Finance
- Regulatory
- REITs
- Securities
- Tax
- Trademarks
- White Collar Defense
---
