---
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: veeva.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: ostrohealth.com
  note: Probed 2026-08-26 with dig — DNSKEY, CAA, TXT (SPF) and _dmarc TXT all returned empty. Ostro's own registrable domain publishes no email-auth or certificate-issuance policy records; TLS 1.3 and HSTS (max-age 31536000) are present on the web listener.
  spf: false
hosts:
- cert_expires: Oct  1 23:54:14 2026 GMT
  host: www.ostrohealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: 301 redirects to ostro.veeva.com
  tls_version: TLSv1.3
- cert_expires: Oct  4 19:02:51 2026 GMT
  host: ostro.veeva.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ostro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ostro, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ostro
provider_slug: ostro
slug: ostro-domain-security
source_filename: ostro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nnote: >-\n  ostro.veeva.com is Ostro's live website host since the March 2026 Veeva\n  Systems acquisition, so its registrable domain (veeva.com) reflects VEEVA's\n  DNS posture, not Ostro's. ostrohealth.com — the domain Ostro registered and\n  still owns, which now 301s to ostro.veeva.com — was probed separately below\n  and carries no SPF, no DMARC, no CAA and no DNSSEC of its own.\nhosts:\n- host: www.ostrohealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:54:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: 301 redirects to ostro.veeva.com\n- host: ostro.veeva.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 19:02:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: veeva.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n\
  \  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: ostrohealth.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  note: >-\n    Probed 2026-08-26 with dig — DNSKEY, CAA, TXT (SPF) and _dmarc TXT all\n    returned empty. Ostro's own registrable domain publishes no email-auth or\n    certificate-issuance policy records; TLS 1.3 and HSTS (max-age 31536000)\n    are present on the web listener.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ostro/refs/heads/main/security/ostro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Life Sciences
- Pharmaceuticals
- Healthcare
- Artificial Intelligence
- Conversational AI
- Patient Engagement
- Marketing
- SaaS
---
