---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: doe.gov
  spf: true
hosts:
- host: edx.netl.doe.gov
  https: false
kind: domain-security
layout: security
method: probed
name: Edx Netl Doe Gov Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DOE NETL Energy Data Exchange, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: DOE NETL Energy Data Exchange
provider_slug: edx-netl-doe-gov
slug: edx-netl-doe-gov-domain-security
source_filename: edx-netl-doe-gov-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: edx.netl.doe.gov\n  https: false\ndomains:\n- domain: doe.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edx-netl-doe-gov/refs/heads/main/security/edx-netl-doe-gov-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Federal Government
- United States
---
