---
api_specs:
- filename: apollo-insurance-affiliates.yml
  format: yaml
  label: APOLLO Affiliates API
  slug: apollo-affiliates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-insurance/refs/heads/main/openapi/apollo-insurance-affiliates.yml
- filename: apollo-insurance-affiliates-legacy.yml
  format: yaml
  label: APOLLO Public API - Affiliates
  slug: apollo-public-api-affiliates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-insurance/refs/heads/main/openapi/apollo-insurance-affiliates-legacy.yml
- filename: apollo-insurance-covertrack.yml
  format: yaml
  label: APOLLO CoverTrack API
  slug: apollo-covertrack-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-insurance/refs/heads/main/openapi/apollo-insurance-covertrack.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apollocover.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: covertrack.ca
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:3917439.spf04.hubspotemail.net ~all
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazonaws.com
  spf: true
hosts:
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: apollocover.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 03:05:30 2026 GMT
  host: docs.apollocover.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  5 23:59:59 2027 GMT
  host: fpl95knwc1.execute-api.ca-central-1.amazonaws.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  4 23:59:59 2027 GMT
  cert_valid: true
  host: api.covertrack.ca
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apollo Insurance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for APOLLO Insurance, probed live across 4 host(s) and 3 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: APOLLO Insurance
provider_slug: apollo-insurance
slug: apollo-insurance-domain-security
source_filename: apollo-insurance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apollocover.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: false\n- host: docs.apollocover.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 03:05:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: fpl95knwc1.execute-api.ca-central-1.amazonaws.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: null\n- host: api.covertrack.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  cert_valid: true\n  hsts: false\ndomains:\n- domain: apollocover.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: covertrack.ca\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 include:_spf.google.com include:3917439.spf04.hubspotemail.net ~all'\n  dmarc: true\n  dmarc_policy: none\n\
  - domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\nfindings:\n  note: >-\n    Recorded observations, not assertions of risk. Added api.covertrack.ca and the covertrack.ca\n    registrable domain in this round — the mechanical probe covered only the apis.yml hosts and\n    the first spec's servers.\n  observations:\n  - No HSTS on apollocover.com or api.covertrack.ca; present only on docs.apollocover.com (max-age 31536000).\n    APOLLO's own security page states \"we leverage browser protections such as HTTP Strict\n    Transport Protection\", which holds for the docs host but not the primary website or the\n    CoverTrack API host.\n  - No CAA records on either apollocover.com or covertrack.ca — any CA may issue for these names.\n  - No DNSSEC on either registrable domain.\n  - DMARC is published on both apollocover.com and covertrack.ca but at 'p=none' — monitoring\n    only, no enforcement against spoofed mail. For a broker that\
  \ emails policy documents to\n    consumers this is the weakest published control.\n  - TLS 1.3 observed on every host, above the TLS 1.2 minimum APOLLO publishes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apollo-insurance/refs/heads/main/security/apollo-insurance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Canada
- Insurtech
- Broker
- Embedded Insurance
- Property and Casualty
- Tenant Insurance
- Quoting
- Distribution
- Compliance
---
