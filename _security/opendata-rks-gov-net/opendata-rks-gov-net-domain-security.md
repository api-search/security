---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rks-gov.net
  spf: true
hosts:
- host: opendata.rks-gov.net
  https: false
kind: domain-security
layout: security
method: probed
name: Opendata Rks Gov Net Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for opendata.rks-gov.net (Kosovo Open Data) [offline], probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: opendata.rks-gov.net (Kosovo Open Data) [offline]
provider_slug: opendata-rks-gov-net
slug: opendata-rks-gov-net-domain-security
source_filename: opendata-rks-gov-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opendata.rks-gov.net\n  https: false\ndomains:\n- domain: rks-gov.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opendata-rks-gov-net/refs/heads/main/security/opendata-rks-gov-net-domain-security.yml
summary_line: DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- Government Data
- National Government
- Kosovo
- Europe
- Offline
---
