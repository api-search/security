---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: creativecommons.engineering
  spf: true
hosts:
- cert_expires: Sep 10 23:53:41 2026 GMT
  host: api.creativecommons.engineering
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Creative Commons Catalog Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Creative Commons Catalog, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Creative Commons Catalog
provider_slug: creative-commons-catalog
slug: creative-commons-catalog-domain-security
source_filename: creative-commons-catalog-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.creativecommons.engineering\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 10 23:53:41 2026 GMT\n  hsts: false\ndomains:\n- domain: creativecommons.engineering\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/creative-commons-catalog/refs/heads/main/security/creative-commons-catalog-domain-security.yml
summary_line: TLSv1.2
tags:
- Open Source Projects
- Public APIs
---
