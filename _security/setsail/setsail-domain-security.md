---
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: setsail.co
  spf: true
hosts:
- cert_expires: Sep 28 06:05:20 2026 GMT
  host: www.setsail.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Setsail Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SetSail, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SetSail
provider_slug: setsail
slug: setsail-domain-security
source_filename: setsail-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.setsail.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 06:05:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: setsail.co\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/setsail/refs/heads/main/security/setsail-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Sales
- Revenue Operations
- RevOps
- Sales Intelligence
- Artificial Intelligence
- CRM
- Salesforce
- Sales Enablement
---
