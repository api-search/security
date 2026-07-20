---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: khoros.ai
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "globalsign.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "sectigo.com"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: khoros.com
  spf: true
hosts:
- cert_expires: Sep  3 05:48:31 2026 GMT
  host: khoros.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 20:18:28 2026 GMT
  host: developer.khoros.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: api.spredfast.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Lithium Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lithium Technologies, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lithium Technologies
provider_slug: lithium-technologies
slug: lithium-technologies-domain-security
source_filename: lithium-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: khoros.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 05:48:31 2026 GMT\n  hsts: false\n- host: developer.khoros.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 20:18:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.spredfast.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: khoros.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: khoros.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lithium-technologies/refs/heads/main/security/lithium-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise Software
- Online Community
- Social Media Management
- Customer Engagement
- Customer Support
- Marketing
- Conversational AI
- Martech
---
