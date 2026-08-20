---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aifi.com
  spf: true
hosts:
- cert_expires: Oct 30 01:23:46 2026 GMT
  host: www.aifi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: auth.aifi.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: Keycloak identity provider (realm `aifi`) fronting the docs and partner portals.
  tls_version: TLSv1.3
- host: docs.aifi.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: Developer documentation portal; every path 302s to the Keycloak login.
  tls_version: TLSv1.3
- host: partners.aifi.com
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 2592000
  https: true
  note: Partner portal single-page application; authenticated.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aifi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AiFi, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AiFi
provider_slug: aifi
slug: aifi-domain-security
source_filename: aifi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aifi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 01:23:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: auth.aifi.com\n  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: Keycloak identity provider (realm `aifi`) fronting the docs and partner portals.\n- host: docs.aifi.com\n  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: Developer documentation portal; every path 302s to the Keycloak login.\n- host: partners.aifi.com\n  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 2592000\n  hsts_include_subdomains: false\n  note: Partner portal single-page application; authenticated.\ndomains:\n- domain: aifi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy:\
  \ reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aifi/refs/heads/main/security/aifi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Computer-Vision
- Retail
- Autonomous Checkout
- Spatial Intelligence
- Artificial Intelligence
- Analytics
- Identity
- Fraud Prevention
- Point-of-Sale
---
