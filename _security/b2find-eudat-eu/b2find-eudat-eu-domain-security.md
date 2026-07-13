---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: eudat.eu
  spf: true
hosts:
- cert_expires: Jan 14 06:31:23 2027 GMT
  host: b2find.eudat.eu
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: B2Find Eudat Eu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EUDAT B2FIND, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: EUDAT B2FIND
provider_slug: b2find-eudat-eu
slug: b2find-eudat-eu-domain-security
source_filename: b2find-eudat-eu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: b2find.eudat.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 06:31:23 2027 GMT\n  hsts: false\ndomains:\n- domain: eudat.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/b2find-eudat-eu/refs/heads/main/security/b2find-eudat-eu-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Organization
- European Union
---
