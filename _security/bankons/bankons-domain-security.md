---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bankons.com
  spf: false
hosts:
- cert_expires: Nov 11 23:14:15 2026 GMT
  host: bankons.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bankons Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BankOns, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: BankOns
provider_slug: bankons
slug: bankons-domain-security
source_filename: bankons-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bankons.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 23:14:15 2026 GMT\n  hsts: false\ndomains:\n- domain: bankons.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\nnotes:\n- bankons.com is a parked GoDaddy lander that returns HTTP 200 for every path (soft-404), so status codes alone\n  are not evidence of a published document. All /.well-known/ probes returned the lander body, not real documents.\ndangling_dns:\n- host: api.bankons.com\n  record: CNAME bankons-api.elasticbeanstalk.com\n  resolves: false\n  connect: failed\n  risk: subdomain-takeover candidate (CNAME to a deleted AWS Elastic Beanstalk environment)\n- host: dev.bankons.com\n  record: CNAME bankons-dev.elasticbeanstalk.com\n  resolves: false\n  connect: failed\n  risk: subdomain-takeover candidate (CNAME to a deleted AWS Elastic Beanstalk environment)\n- host:\
  \ docs.bankons.com\n  record: CNAME ghs.google.com\n  resolves: true\n  http_status: 404\n  risk: dangling CNAME to unclaimed Google-hosted site\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bankons/refs/heads/main/security/bankons-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Defunct
- Acquired
- Financial Services
- Fintech
- Mobile
- Personal Finance
- Rewards
- Deals
- Consumer
---
