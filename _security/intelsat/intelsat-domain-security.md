---
api_specs:
- filename: intelsat-openapi-generated.yml
  format: yaml
  label: Intelsat API
  slug: intelsat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelsat/refs/heads/main/openapi/_ae-authored/intelsat-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: intelsat.com
  spf: true
hosts:
- cert_expires: Dec 17 02:54:26 2026 GMT
  host: intelsat.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Intelsat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Intelsat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Intelsat
provider_slug: intelsat
slug: intelsat-domain-security
source_filename: intelsat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: intelsat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 02:54:26 2026 GMT\n  hsts: false\ndomains:\n- domain: intelsat.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intelsat/refs/heads/main/security/intelsat-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Satellite
- Communications
- Connectivity
- Enterprise
- Media
---
