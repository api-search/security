---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: niagaraopendata.ca
  spf: true
hosts:
- cert_expires: Sep 25 21:45:45 2026 GMT
  host: niagaraopendata.ca
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Niagaraopendata Ca Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Niagara Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Niagara Open Data
provider_slug: niagaraopendata-ca
slug: niagaraopendata-ca-domain-security
source_filename: niagaraopendata-ca-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: niagaraopendata.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 21:45:45 2026 GMT\n  hsts: false\ndomains:\n- domain: niagaraopendata.ca\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/niagaraopendata-ca/refs/heads/main/security/niagaraopendata-ca-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- County Government
- Canada
---
