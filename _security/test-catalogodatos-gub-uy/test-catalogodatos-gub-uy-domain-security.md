---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: gub.uy
  spf: false
hosts:
- cert_expires: Aug 18 11:28:54 2026 GMT
  host: test.catalogodatos.gub.uy
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Test Catalogodatos Gub Uy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Uruguay Open Data Catalogue, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Uruguay Open Data Catalogue
provider_slug: test-catalogodatos-gub-uy
slug: test-catalogodatos-gub-uy-domain-security
source_filename: test-catalogodatos-gub-uy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: test.catalogodatos.gub.uy\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 18 11:28:54 2026 GMT\n  hsts: false\ndomains:\n- domain: gub.uy\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/test-catalogodatos-gub-uy/refs/heads/main/security/test-catalogodatos-gub-uy-domain-security.yml
summary_line: TLSv1.2 · DNSSEC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- National Government
- Uruguay
---
