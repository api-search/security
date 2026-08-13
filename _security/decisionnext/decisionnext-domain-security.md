---
description: ''
domains:
- caa:
  - 0 issuewild "godaddy.com"
  - 0 iodef "mailto:operations@decisionnext.com"
  - 0 issue "amazon.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: decisionnext.com
  spf: true
hosts:
- cert_expires: Feb 12 23:59:59 2027 GMT
  host: decisionnext.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Decisionnext Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DecisionNext, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DecisionNext
provider_slug: decisionnext
slug: decisionnext-domain-security
source_filename: decisionnext-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: decisionnext.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: decisionnext.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"godaddy.com\"\n  - 0 iodef \"mailto:operations@decisionnext.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/decisionnext/refs/heads/main/security/decisionnext-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Analytics
- Artificial Intelligence
- Machine Learning
- Forecasting
- Commodities
- Agriculture
- Food and Beverage
- Mining and Natural Resources
- Supply Chain
- Procurement
- Pricing
- Risk Management
- Decision Support
- SaaS
---
