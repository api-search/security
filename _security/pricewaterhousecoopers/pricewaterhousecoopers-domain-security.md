---
description: ''
domains:
- caa:
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pwc.com
  spf: true
hosts:
- cert_expires: Jul 30 15:37:14 2026 GMT
  host: www.pwc.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pricewaterhousecoopers Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PwC (PricewaterhouseCoopers), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PwC (PricewaterhouseCoopers)
provider_slug: pricewaterhousecoopers
slug: pricewaterhousecoopers-domain-security
source_filename: pricewaterhousecoopers-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pwc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 30 15:37:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pwc.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pricewaterhousecoopers/refs/heads/main/security/pricewaterhousecoopers-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Consulting
- Audit
- Assurance
- Tax
- Advisory
- Professional Services
- Big Four
- Risk
- Deals
- Technology
- AI
- Generative AI
- Research
- Insights
- Industry Analysis
- ESG
- Workforce
---
