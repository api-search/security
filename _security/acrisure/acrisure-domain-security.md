---
description: ''
domains:
- caa: []
  caa_note: No CAA record is published, so any public CA may issue for this domain.
  dmarc: true
  dmarc_alignment: strict (adkim=s, aspf=s)
  dmarc_note: p=quarantine rather than p=reject, so spoofed mail is junked rather than rejected outright.
  dmarc_pct: 100
  dmarc_policy: quarantine
  dmarc_reporting: Aggregate reports to Cloudflare, security@acrisure.com and EasyDMARC; forensic reports to EasyDMARC.
  dmarc_subdomain_policy: quarantine
  dnssec: true
  domain: acrisure.com
  spf: true
hosts:
- cert_expires: Sep 24 04:19:52 2026 GMT
  host: www.acrisure.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 04:19:52 2026 GMT
  host: api.acrisure.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: Observed on GET /.well-known/security.txt (200). The automated probe recorded null because this host's root is answered by a Cloudflare WAF block; the header is present on both the block page and on origin responses.
  tls_version: TLSv1.3
- host: customer.acrisure.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: Customer portal SPA in front of a Spring Boot service. Added manually — it was not in apis.yml when the automated probe ran.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Acrisure Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acrisure, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Acrisure
provider_slug: acrisure
slug: acrisure-domain-security
source_filename: acrisure-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + discovered API hosts\nhosts:\n- host: www.acrisure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 04:19:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.acrisure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 04:19:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: >-\n    Observed on GET /.well-known/security.txt (200). The automated probe recorded null\n    because this host's root is answered by a Cloudflare WAF block; the header is present\n    on both the block page and on origin responses.\n- host: customer.acrisure.com\n  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: >-\n    Customer portal SPA in front of a Spring Boot service. Added manually — it was not in\n    apis.yml when the automated probe ran.\ndomains:\n\
  - domain: acrisure.com\n  dnssec: true\n  caa: []\n  caa_note: No CAA record is published, so any public CA may issue for this domain.\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_subdomain_policy: quarantine\n  dmarc_alignment: strict (adkim=s, aspf=s)\n  dmarc_pct: 100\n  dmarc_reporting: >-\n    Aggregate reports to Cloudflare, security@acrisure.com and EasyDMARC; forensic reports\n    to EasyDMARC.\n  dmarc_note: >-\n    p=quarantine rather than p=reject, so spoofed mail is junked rather than rejected\n    outright.\nx-evidence:\n  fetched: '2026-08-06'\n  probes:\n  - url: https://api.acrisure.com/.well-known/security.txt\n    http_status: 200\n    header: 'strict-transport-security: max-age=31536000; includeSubDomains'\n  - url: https://customer.acrisure.com/.well-known/security.txt\n    http_status: 200\n    header: 'strict-transport-security: max-age=31536000; includeSubDomains'\n  - query: CAA acrisure.com\n    result: empty\n  - query: TXT _dmarc.acrisure.com\n\
  \    result: 'v=DMARC1; p=quarantine; sp=quarantine; adkim=s; aspf=s; pct=100'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acrisure/refs/heads/main/security/acrisure-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Insurance
- Insurance Brokerage
- Fintech
- Employee Benefits
- payroll-hr
- Reinsurance
- Risk Management
- Cybersecurity
- Mortgage
- Surety Bonds
- MCP
- Authentication
---
