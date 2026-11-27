---
api_specs:
- filename: aboard-sh-openapi-generated.yml
  format: yaml
  label: Aboard API
  slug: aboard-sh-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aboard-sh/openapi/_ae-authored/aboard-sh-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aboard.sh
  spf: true
hosts:
- cert_expires: Jan 20 19:05:06 2027 GMT
  host: aboard.sh
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aboard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aboard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Aboard
provider_slug: aboard-sh
slug: aboard-sh-domain-security
source_filename: aboard-sh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aboard.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 19:05:06 2027 GMT\n  hsts: false\ndomains:\n- domain: aboard.sh\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/aboard-sh/security/aboard-sh-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Collaboration
- Chat
- Agents
- Platform
---
