---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dechert.com
  spf: true
hosts:
- cert_expires: Jan  4 23:59:59 2027 GMT
  host: www.dechert.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dechert Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dechert, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dechert
provider_slug: dechert
slug: dechert-domain-security
source_filename: dechert-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dechert.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: dechert.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dechert/refs/heads/main/security/dechert-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Antitrust
- Arbitration
- Artificial Intelligence
- Asset Management
- Banking
- CLOs
- Competition
- Corporate
- Crisis Management
- Cryptocurrency
- Cybersecurity
- Data Privacy
- Employee Benefits
- Enforcement
- ESG
- Financial Restructuring
- Financial Services
- Fintech
- Global Finance
- Government Contracts
- Intellectual Property
- International Arbitration
- Investigations
- Investment Management
- Law
- Law Firm
- Legal
- Legal Services
- Life Sciences
- Litigation
- Mergers and Acquisitions
- National Security
- Permanent Capital
- Pharmaceuticals
- Private Client
- Private Credit
- Private Equity
- Product Liability
- Real Estate
- Regulatory
- Sovereign Wealth Funds
- Sustainability
- Tax
- White Collar
---
