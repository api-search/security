---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cardless.com
  spf: true
hosts:
- cert_expires: Sep  7 10:39:46 2026 GMT
  host: www.cardless.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 11:02:22 2026 GMT
  host: docs.cardless.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: api.cardless.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cardless Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cardless, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cardless
provider_slug: cardless
slug: cardless-domain-security
source_filename: cardless-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cardless.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 10:39:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.cardless.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 11:02:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.cardless.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: cardless.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cardless/refs/heads/main/security/cardless-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Services
- Fintech
- Credit Cards
- Card Issuing
- Embedded Finance
- Payments
- Banking as a Service
- Lending
- Co-Branded Cards
- Loyalty
---
