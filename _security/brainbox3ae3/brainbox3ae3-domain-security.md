---
api_specs:
- filename: brainbox3ae3-openapi-generated.yml
  format: yaml
  label: Brainbox3ae3 API
  slug: brainbox3ae3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brainbox3ae3/refs/heads/main/openapi/_ae-authored/brainbox3ae3-openapi-generated.yml
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
  dmarc_policy: reject
  dnssec: false
  domain: brainboxes.com
  spf: true
hosts:
- cert_expires: Nov 30 12:28:15 2026 GMT
  host: www.brainboxes.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Brainbox3Ae3 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brainbox3ae3, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Brainbox3ae3
provider_slug: brainbox3ae3
slug: brainbox3ae3-domain-security
source_filename: brainbox3ae3-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.brainboxes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 12:28:15 2026 GMT\n  hsts: false\ndomains:\n- domain: brainboxes.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brainbox3ae3/refs/heads/main/security/brainbox3ae3-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Industrial
- Connectivity
- IoT
- Automation
---
