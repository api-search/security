---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: falconfs.com
  spf: true
hosts:
- cert_expires: Sep 16 20:54:38 2026 GMT
  host: falconfs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 20:35:46 2026 GMT
  host: docs.falconfs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 16 11:07:03 2027 GMT
  host: credituat.falconfs.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Falcon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Falcon, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Falcon
provider_slug: falcon
slug: falcon-domain-security
source_filename: falcon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: falconfs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 20:54:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.falconfs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 20:35:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: credituat.falconfs.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 16 11:07:03 2027 GMT\n  hsts: null\ndomains:\n- domain: falconfs.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/falcon/refs/heads/main/security/falcon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Infrastructure
- Financial Services
- Banking
- Payments
- Credit Cards
- Embedded Finance
- Fintech
- Card Issuing
- Lending
- Banking as a Service
- India
---
