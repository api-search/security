---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: service.gov.uk
  spf: true
hosts:
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: ckan.publishing.service.gov.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ckan Publishing Service Gov Uk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for data.gov.uk CKAN Publishing Service, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: data.gov.uk CKAN Publishing Service
provider_slug: ckan-publishing-service-gov-uk
slug: ckan-publishing-service-gov-uk-domain-security
source_filename: ckan-publishing-service-gov-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ckan.publishing.service.gov.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: service.gov.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ckan-publishing-service-gov-uk/refs/heads/main/security/ckan-publishing-service-gov-uk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- National Government
- United Kingdom
---
