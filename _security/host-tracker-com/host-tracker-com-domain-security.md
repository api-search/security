---
api_specs:
- filename: host-tracker-com-openapi-generated.yml
  format: yaml
  label: HostTracker API
  slug: host-tracker-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/host-tracker-com/openapi/_ae-authored/host-tracker-com-openapi-generated.yml
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
  dmarc_policy: quarantine
  dnssec: false
  domain: host-tracker.com
  spf: true
hosts:
- cert_expires: Feb  2 02:35:58 2027 GMT
  host: host-tracker.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: HostTracker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HostTracker, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: HostTracker
provider_slug: host-tracker-com
slug: host-tracker-com-domain-security
source_filename: host-tracker-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: host-tracker.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 02:35:58 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: host-tracker.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/host-tracker-com/security/host-tracker-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Monitoring
- Uptime
- Websites
- Alerts
- Software-as-a-Service
---
