---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: essex.gov.uk
  spf: true
hosts:
- cert_expires: Aug 18 21:48:07 2026 GMT
  host: data.essex.gov.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Data Essex Gov Uk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Essex Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Essex Open Data
provider_slug: data-essex-gov-uk
slug: data-essex-gov-uk-domain-security
source_filename: data-essex-gov-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.essex.gov.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 21:48:07 2026 GMT\n  hsts: null\ndomains:\n- domain: essex.gov.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/data-essex-gov-uk/refs/heads/main/security/data-essex-gov-uk-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Local Council
- United Kingdom
---
