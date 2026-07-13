---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: opendata.com.pk
  spf: true
hosts:
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: opendata.com.pk
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Opendata Com Pk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pakistan Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pakistan Open Data
provider_slug: opendata-com-pk
slug: opendata-com-pk-domain-security
source_filename: opendata-com-pk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opendata.com.pk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: opendata.com.pk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opendata-com-pk/refs/heads/main/security/opendata-com-pk-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- National Government
- Pakistan
---
