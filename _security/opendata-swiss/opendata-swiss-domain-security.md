---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: opendata.swiss
  spf: true
hosts:
- cert_expires: Sep 14 11:54:44 2026 GMT
  host: opendata.swiss
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opendata Swiss Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for opendata.swiss, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: opendata.swiss
provider_slug: opendata-swiss
slug: opendata-swiss-domain-security
source_filename: opendata-swiss-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opendata.swiss\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 11:54:44 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: opendata.swiss\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opendata-swiss/refs/heads/main/security/opendata-swiss-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- National Government
- Switzerland
---
