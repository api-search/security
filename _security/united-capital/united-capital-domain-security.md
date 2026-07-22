---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dmarc_record: v=DMARC1; p=none; rua=mailto:postmaster@unitedcp.com; ruf=mailto:postmaster@unitedcp.com; fo=0; adkim=r; aspf=r; pct=100; ri=86400; sp=none
  dnssec: false
  domain: unitedcp.com
  mx:
  - 0 unitedcp-com.mail.protection.outlook.com.
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:_spf.salesforce.com include:cust-spf.exacttarget.com ip4:207.99.52.203 ip4:18.204.183.4 include:aspmx.pardot.com include:spf.protection.outlook.com ~all
hosts:
- cert_expires: Aug 29 20:15:00 2026 GMT
  cert_issuer: C=US, O=Google Trust Services, CN=WE1
  host: unitedcp.com
  hsts: false
  http_status: 404
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: United Capital Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for United Capital, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: United Capital
provider_slug: united-capital
slug: united-capital-domain-security
source_filename: united-capital-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of the historic company domain (unitedcp.com)\nnote: >-\n  United Capital Financial Advisers was acquired by Goldman Sachs in 2019 and no\n  longer operates independently. The website returns HTTP 404 (UltraDNS parking\n  behind Cloudflare), but the domain still resolves, serves TLS, and carries live\n  mail (MX/SPF/DMARC) records — probed here as the historic corporate domain.\nhosts:\n- host: unitedcp.com\n  https: true\n  http_status: 404\n  tls_version: TLSv1.3\n  cert_issuer: 'C=US, O=Google Trust Services, CN=WE1'\n  cert_expires: Aug 29 20:15:00 2026 GMT\n  hsts: false\ndomains:\n- domain: unitedcp.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 include:_spf.google.com include:_spf.salesforce.com include:cust-spf.exacttarget.com ip4:207.99.52.203 ip4:18.204.183.4 include:aspmx.pardot.com include:spf.protection.outlook.com ~all'\n  dmarc: true\n  dmarc_policy: none\n  dmarc_record:\
  \ 'v=DMARC1; p=none; rua=mailto:postmaster@unitedcp.com; ruf=mailto:postmaster@unitedcp.com; fo=0; adkim=r; aspf=r; pct=100; ri=86400; sp=none'\n  mx:\n  - 0 unitedcp-com.mail.protection.outlook.com.\nwell_known:\n- path: /.well-known/security.txt\n  status: 404\n- path: /.well-known/openid-configuration\n  status: 404\n- path: /.well-known/oauth-authorization-server\n  status: 404\n- path: /.well-known/api-catalog\n  status: 404\n- path: /.well-known/ai-plugin.json\n  status: 404\n- path: /llms.txt\n  status: 404\n- path: /robots.txt\n  status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/united-capital/refs/heads/main/security/united-capital-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Wealth Management
- Financial Advisors
- Financial Planning
- Acquired
---
