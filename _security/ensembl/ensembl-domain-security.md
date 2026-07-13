---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ensembl.org
  spf: true
hosts:
- cert_expires: Nov 16 09:53:18 2026 GMT
  host: www.ensembl.org
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 16 09:53:18 2026 GMT
  host: rest.ensembl.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ensembl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ensembl, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Ensembl
provider_slug: ensembl
slug: ensembl-domain-security
source_filename: ensembl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ensembl.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 09:53:18 2026 GMT\n  hsts: null\n- host: rest.ensembl.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 09:53:18 2026 GMT\n  hsts: false\ndomains:\n- domain: ensembl.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ensembl/refs/heads/main/security/ensembl-domain-security.yml
summary_line: TLSv1.3
tags:
- Genomics
- Bioinformatics
- Genome Annotation
- Variant Annotation
- Comparative Genomics
- Life Sciences
- REST API
---
