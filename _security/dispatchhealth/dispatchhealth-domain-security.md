---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: dispatchhealth.com
  spf: true
hosts:
- cert_expires: Sep 21 03:08:15 2026 GMT
  host: www.dispatchhealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 14:01:31 2026 GMT
  host: api.dispatchhealth.com
  hsts: null
  https: true
  note: responds HTTP 204 with an empty body to every path probed (no public contract surface); AWS ELB/Traefik ingress
  tls_version: TLSv1.3
- cert_expires: Oct  9 23:59:59 2026 GMT
  host: express.dispatchhealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 23:59:59 2026 GMT
  host: request.dispatchhealth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 23:59:59 2026 GMT
  host: portal.dispatchhealth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 14:31:52 2026 GMT
  host: careers.dispatchhealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  7 19:01:30 2026 GMT
  host: trust.dispatchhealth.com
  hsts: null
  https: true
  note: Drata-hosted trust center (CNAME trust.cname.drata.com) behind a Cloudflare bot challenge
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dispatchhealth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DispatchHealth, probed live across 7 host(s) and 1 registrable domain(s). 7 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: DispatchHealth
provider_slug: dispatchhealth
slug: dispatchhealth-domain-security
source_filename: dispatchhealth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + subdomain hosts\nhosts:\n- host: www.dispatchhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 03:08:15 2026 GMT\n  hsts: false\n- host: api.dispatchhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 14:01:31 2026 GMT\n  hsts: null\n  note: responds HTTP 204 with an empty body to every path probed (no public contract\n    surface); AWS ELB/Traefik ingress\n- host: express.dispatchhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 23:59:59 2026 GMT\n  hsts: false\n- host: request.dispatchhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: portal.dispatchhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: careers.dispatchhealth.com\n  https: true\n\
  \  tls_version: TLSv1.2\n  cert_expires: Sep  7 14:31:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: trust.dispatchhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 19:01:30 2026 GMT\n  hsts: null\n  note: Drata-hosted trust center (CNAME trust.cname.drata.com) behind a Cloudflare\n    bot challenge\ndomains:\n- domain: dispatchhealth.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dispatchhealth/refs/heads/main/security/dispatchhealth-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Health Systems
- Hospital at Home
- Home Health
- Urgent Care
- Care Delivery
- Medical Services
- Telehealth
- Digital Health
---
