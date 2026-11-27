---
api_specs:
- filename: kleap-co-account-api-openapi.yml
  format: yaml
  label: Kleap Account API
  slug: kleap-co-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kleap-co/openapi/kleap-co-account-api-openapi.yml
- filename: kleap-co-apps-api-openapi.yml
  format: yaml
  label: Kleap Apps API
  slug: kleap-co-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kleap-co/openapi/kleap-co-apps-api-openapi.yml
- filename: kleap-co-auth-api-openapi.yml
  format: yaml
  label: Kleap Auth API
  slug: kleap-co-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kleap-co/openapi/kleap-co-auth-api-openapi.yml
- filename: kleap-co-tasks-api-openapi.yml
  format: yaml
  label: Kleap Tasks API
  slug: kleap-co-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kleap-co/openapi/kleap-co-tasks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kleap.co
  spf: true
hosts:
- cert_expires: Jan 23 20:33:07 2027 GMT
  host: kleap.co
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kleap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kleap, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kleap
provider_slug: kleap-co
slug: kleap-co-domain-security
source_filename: kleap-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kleap.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 20:33:07 2027 GMT\n  hsts: false\ndomains:\n- domain: kleap.co\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/kleap-co/security/kleap-co-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Website Builder
- No-Code
- Entrepreneurship
- Software-as-a-Service
---
