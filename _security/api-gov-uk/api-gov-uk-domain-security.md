---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: api.gov.uk
  spf: true
hosts:
- cert_expires: Jan 16 18:33:22 2027 GMT
  host: www.api.gov.uk
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: UK Government API Catalogue Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UK Government API Catalogue, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: UK Government API Catalogue
provider_slug: api-gov-uk
slug: api-gov-uk-domain-security
source_filename: api-gov-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.api.gov.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 18:33:22 2027 GMT\n  hsts: false\ndomains:\n- domain: api.gov.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/api-gov-uk/security/api-gov-uk-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Government
- United Kingdom
- API Catalog
- API Discovery
- Directory
- Open Data
---
