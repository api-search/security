---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cyberresilience.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: resilienceinsurance.app
  note: Registrable domain of the private product API. DMARC is p=none (monitor only) and reports to dmarc@resilienceinsurance.com. Hand-probed 2026-07-25.
  spf: true
hosts:
- cert_expires: Oct 14 23:22:41 2026 GMT
  host: cyberresilience.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: portal.cyberresilience.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 18:22:06 2026 GMT
  host: auth.cyberresilience.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 00:42:42 2026 GMT
  host: trust.cyberresilience.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: Vanta-hosted trust center; hand-probed 2026-07-25 (not in apis.yml host set).
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: api.prod.resilienceinsurance.app
  hsts: false
  http_status: 404
  https: true
  note: Private product API named as the OAuth audience. Serves a valid certificate but 404s anonymously and sends no HSTS header. Hand-probed 2026-07-25.
kind: domain-security
layout: security
method: probed
name: Resilience Cyber Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Resilience, probed live across 5 host(s) and 2 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Resilience
provider_slug: resilience-cyber
slug: resilience-cyber-domain-security
source_filename: resilience-cyber-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cyberresilience.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:22:41 2026 GMT\n  hsts: false\n- host: portal.cyberresilience.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: null\n- host: auth.cyberresilience.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 18:22:06 2026 GMT\n  hsts: false\n- host: trust.cyberresilience.com\n  https: true\n  cert_expires: Sep 26 00:42:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: Vanta-hosted trust center; hand-probed 2026-07-25 (not in apis.yml host set).\n- host: api.prod.resilienceinsurance.app\n  https: true\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: false\n  http_status: 404\n  note: >-\n    Private product API named as the OAuth audience. Serves a valid certificate\n    but 404s\
  \ anonymously and sends no HSTS header. Hand-probed 2026-07-25.\ndomains:\n- domain: cyberresilience.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: resilienceinsurance.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  note: >-\n    Registrable domain of the private product API. DMARC is p=none (monitor\n    only) and reports to dmarc@resilienceinsurance.com. Hand-probed 2026-07-25.\nfindings:\n- >-\n  No CAA records on either registrable domain — certificate issuance is not\n  constrained to named CAs.\n- >-\n  No DNSSEC on either registrable domain.\n- >-\n  HSTS is present only on the Vanta-hosted trust center; the marketing site, the\n  Auth0 tenant host and the product API host send no Strict-Transport-Security\n  header.\n- >-\n  cyberresilience.com DMARC is p=quarantine; resilienceinsurance.app DMARC is\n  p=none.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/resilience-cyber/refs/heads/main/security/resilience-cyber-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- United States
- Cyber Insurance
- Property and Casualty
- Insurtech
- Underwriting
- Claims
- Risk Data
- Technology Errors and Omissions
- Broker
- Specialty Insurance
---
