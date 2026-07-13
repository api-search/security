---
api_specs:
- filename: api
  format: yaml
  label: UniProtKB REST API
  slug: uniprotkb-rest-api
  spec_type: OpenAPI
  url: https://www.uniprot.org/help/api
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: uniprot.org
  spf: true
hosts:
- cert_expires: Oct 20 22:06:56 2026 GMT
  host: www.uniprot.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 22:06:56 2026 GMT
  host: rest.uniprot.org
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 08:14:01 2026 GMT
  host: sparql.uniprot.org
  hsts: true
  hsts_max_age: 31536001
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uniprot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UniProt, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: UniProt
provider_slug: uniprot
slug: uniprot-domain-security
source_filename: uniprot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.uniprot.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 22:06:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: rest.uniprot.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 22:06:56 2026 GMT\n  hsts: null\n- host: sparql.uniprot.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 08:14:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536001\ndomains:\n- domain: uniprot.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uniprot/refs/heads/main/security/uniprot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Proteins
- Bioinformatics
- Genomics
- Life Sciences
- Open Data
---
