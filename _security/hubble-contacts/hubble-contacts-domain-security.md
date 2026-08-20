---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_note: DMARC policy is p=none — monitoring only. Neither quarantine nor reject is enforced, so spoofed mail from hubblecontacts.com is not rejected by receivers.
  dmarc_policy: none
  dnssec: false
  domain: hubblecontacts.com
  spf: true
hosts:
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: www.hubblecontacts.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 00:04:02 2026 GMT
  host: account.hubblecontacts.com
  hsts: true
  hsts_max_age: 7889238
  hsts_note: 'The mechanical probe recorded null; a direct HEAD and GET of https://account.hubblecontacts.com/ and /products.json both returned "strict-transport-security: max-age=7889238" on 2026-08-04, so the value is corrected here from direct observation. Note max-age is ~91 days, below the 31536000 (1 year) HSTS preload threshold, and no includeSubDomains or preload directive is set.'
  https: true
  tls_version: TLSv1.3
- host: api.hubblecontacts.com
  https: true
  note: Resolves and answers, but serves a Rails application shell with no discoverable API contract; every spec and /.well-known/ path probed returned 404.
  probed: true
kind: domain-security
layout: security
method: probed
name: Hubble Contacts Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hubble Contacts, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hubble Contacts
provider_slug: hubble-contacts
slug: hubble-contacts-domain-security
source_filename: hubble-contacts-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hubblecontacts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: null\n- host: account.hubblecontacts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 00:04:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\n  hsts_note: >-\n    The mechanical probe recorded null; a direct HEAD and GET of\n    https://account.hubblecontacts.com/ and /products.json both returned\n    \"strict-transport-security: max-age=7889238\" on 2026-08-04, so the value is\n    corrected here from direct observation. Note max-age is ~91 days, below the\n    31536000 (1 year) HSTS preload threshold, and no includeSubDomains or preload\n    directive is set.\n- host: api.hubblecontacts.com\n  https: true\n  probed: true\n  note: >-\n    Resolves and answers, but serves a Rails application shell with no discoverable\n    API\
  \ contract; every spec and /.well-known/ path probed returned 404.\ndomains:\n- domain: hubblecontacts.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dmarc_note: >-\n    DMARC policy is p=none — monitoring only. Neither quarantine nor reject is\n    enforced, so spoofed mail from hubblecontacts.com is not rejected by receivers.\ngaps:\n- no CAA record on hubblecontacts.com\n- no DNSSEC on hubblecontacts.com\n- DMARC policy is p=none rather than quarantine or reject\n- no HSTS header on www.hubblecontacts.com (present only on the storefront host)\n- no /.well-known/security.txt on any host (see security/ vulnerability disclosure)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hubble-contacts/refs/heads/main/security/hubble-contacts-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- E-Commerce
- Retail
- Health
- Vision Care
- Contact Lenses
- Subscription
- Agentic Commerce
- MCP
- Shopify
- GraphQL
---
