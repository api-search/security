---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: neolaiacampus.eu
  spf: true
hosts:
- cert_expires: Sep 14 23:30:56 2026 GMT
  host: data.neolaiacampus.eu
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Data Neolaiacampus Eu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Neolaiacampus Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Neolaiacampus Open Data
provider_slug: data-neolaiacampus-eu
slug: data-neolaiacampus-eu-domain-security
source_filename: data-neolaiacampus-eu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.neolaiacampus.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 23:30:56 2026 GMT\n  hsts: false\ndomains:\n- domain: neolaiacampus.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/data-neolaiacampus-eu/refs/heads/main/security/data-neolaiacampus-eu-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Organization
- Europe
---
