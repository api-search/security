---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: trento.it
  spf: false
hosts:
- cert_expires: Sep 30 09:04:35 2026 GMT
  host: opendata.comune.trento.it
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opendata Comune Trento It Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trento Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Trento Open Data
provider_slug: opendata-comune-trento-it
slug: opendata-comune-trento-it-domain-security
source_filename: opendata-comune-trento-it-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opendata.comune.trento.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 09:04:35 2026 GMT\n  hsts: false\ndomains:\n- domain: trento.it\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opendata-comune-trento-it/refs/heads/main/security/opendata-comune-trento-it-domain-security.yml
summary_line: TLSv1.3
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Municipal Government
- Italy
---
