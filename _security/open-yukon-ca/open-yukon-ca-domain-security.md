---
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: yukon.ca
  spf: true
hosts:
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: open.yukon.ca
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Yukon Ca Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yukon Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Yukon Open Data
provider_slug: open-yukon-ca
slug: open-yukon-ca-domain-security
source_filename: open-yukon-ca-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: open.yukon.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: yukon.ca\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-yukon-ca/refs/heads/main/security/open-yukon-ca-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Territorial Government
- Canada
---
