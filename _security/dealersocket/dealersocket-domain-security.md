---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog cansignhttpexchanges=yes"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dealersocket.com
  spf: true
hosts:
- cert_expires: Sep 13 04:59:18 2026 GMT
  host: dealersocket.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dealersocket Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DealerSocket, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DealerSocket
provider_slug: dealersocket
slug: dealersocket-domain-security
source_filename: dealersocket-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dealersocket.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 04:59:18 2026 GMT\n  hsts: false\ndomains:\n- domain: dealersocket.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog cansignhttpexchanges=yes\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dealersocket/refs/heads/main/security/dealersocket-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Automotive
- Dealership
- CRM
- DMS
- Leads
- Inventory
- Deals
- Solera
- Partner API
- Certified Partners
---
