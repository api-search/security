---
api_specs:
- filename: fortnite-tracker.yaml
  format: yaml
  label: Fortnite Tracker
  slug: fortnite-tracker
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fortnite/refs/heads/main/openapi/fortnite-tracker.yaml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fortnitetracker.com
  spf: true
hosts:
- cert_expires: Aug 21 10:39:23 2026 GMT
  host: fortnitetracker.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.fortnitetracker.com
  https: false
kind: domain-security
layout: security
method: probed
name: Fortnite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fortnite Tracker, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Fortnite Tracker
provider_slug: fortnite
slug: fortnite-domain-security
source_filename: fortnite-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fortnitetracker.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 10:39:23 2026 GMT\n  hsts: null\n- host: api.fortnitetracker.com\n  https: false\ndomains:\n- domain: fortnitetracker.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fortnite/refs/heads/main/security/fortnite-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Games And Comics
- Public APIs
- Fortnite
- Player Statistics
- Esports
- Tracker Network
---
