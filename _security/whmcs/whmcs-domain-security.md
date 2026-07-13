---
api_specs:
- filename: whmcs-openapi.yml
  format: yaml
  label: WHMCS API
  slug: whmcs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whmcs/main/openapi/whmcs-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: whmcs.com
  spf: true
hosts:
- cert_expires: Aug 13 23:18:12 2026 GMT
  host: www.whmcs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 06:40:00 2026 GMT
  host: developers.whmcs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Whmcs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WHMCS, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: WHMCS
provider_slug: whmcs
slug: whmcs-domain-security
source_filename: whmcs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.whmcs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 23:18:12 2026 GMT\n  hsts: false\n- host: developers.whmcs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 06:40:00 2026 GMT\n  hsts: false\ndomains:\n- domain: whmcs.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whmcs/refs/heads/main/security/whmcs-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Web Hosting
- Billing Automation
- Client Management
- Domain Management
- Support Tickets
- Provisioning
---
