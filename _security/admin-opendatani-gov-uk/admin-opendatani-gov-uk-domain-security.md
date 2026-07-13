---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: opendatani.gov.uk
  spf: true
hosts:
- cert_expires: Sep 17 06:50:23 2026 GMT
  host: admin.opendatani.gov.uk
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Admin Opendatani Gov Uk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenDataNI (Northern Ireland), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: OpenDataNI (Northern Ireland)
provider_slug: admin-opendatani-gov-uk
slug: admin-opendatani-gov-uk-domain-security
source_filename: admin-opendatani-gov-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: admin.opendatani.gov.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 06:50:23 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: opendatani.gov.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/admin-opendatani-gov-uk/refs/heads/main/security/admin-opendatani-gov-uk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Regional Government
- United Kingdom
---
