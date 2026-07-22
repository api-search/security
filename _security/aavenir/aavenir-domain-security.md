---
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aavenir.com
  spf: true
hosts:
- cert_expires: Sep  8 03:02:32 2026 GMT
  host: www.aavenir.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aavenir Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aavenir, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Aavenir
provider_slug: aavenir
slug: aavenir-domain-security
source_filename: aavenir-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aavenir.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 03:02:32 2026 GMT\n  hsts: null\ndomains:\n- domain: aavenir.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aavenir/refs/heads/main/security/aavenir-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Cloud Saas
- Contract Lifecycle Management
- Procurement
- Source To Pay
- Workflow Automation
- ServiceNow
- Artificial Intelligence
- Legal Tech
---
