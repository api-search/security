---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: credit-agricole.fr
  spf: true
hosts:
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: www.credit-agricole.fr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Credit Agricole Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Credit Agricole, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Credit Agricole
provider_slug: credit-agricole
slug: credit-agricole-domain-security
source_filename: credit-agricole-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.credit-agricole.fr\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: credit-agricole.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/credit-agricole/refs/heads/main/security/credit-agricole-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Banking
- Finance
- France
- Retail
---
