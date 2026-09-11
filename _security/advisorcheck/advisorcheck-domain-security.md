---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: advisorcheck.com
  spf: true
hosts:
- cert_expires: Nov  3 01:56:51 2026 GMT
  host: www.advisorcheck.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 29 23:59:59 2026 GMT
  host: api.advisorcheck.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Advisorcheck Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AdvisorCheck, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AdvisorCheck
provider_slug: advisorcheck
slug: advisorcheck-domain-security
source_filename: advisorcheck-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.advisorcheck.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 01:56:51 2026 GMT\n  hsts: null\n- host: api.advisorcheck.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: advisorcheck.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\nnote: Probed 2026-09-09. Neither host sets Strict-Transport-Security (no HSTS on the Vercel front end\n  or the AWS API Gateway host). advisorcheck.com publishes NO DNSSEC and NO CAA record, and DMARC is present\n  but set to p=none (monitor only, no enforcement). DNS also carries THREE conflicting v=spf1 TXT records\n  (Outlook/SES, Zoho One, Zoho zcsend) — RFC 7208 permits exactly one, so receivers must return permerror\n  and SPF is effectively unenforceable on this domain. www.advisorcheck.com is Vercel\
  \ (cname.vercel-dns.com);\n  api.advisorcheck.com is an AWS API Gateway custom domain; help.advisorcheck.com is Gleap (customers.gleap.help).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/advisorcheck/refs/heads/main/security/advisorcheck-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Financial Services
- Fintech
- Regulatory Data
- Background Checks
- Investor Protection
- Financial Advisors
- Wealth Management
- Consumer Finance
- Compliance
---
