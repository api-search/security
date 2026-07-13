---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: leedsdatamill.org
  spf: false
hosts:
- cert_expires: Aug 31 20:27:56 2026 GMT
  host: leedsdatamill.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Leedsdatamill Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Leeds Data Mill, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Leeds Data Mill
provider_slug: leedsdatamill-org
slug: leedsdatamill-org-domain-security
source_filename: leedsdatamill-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: leedsdatamill.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 20:27:56 2026 GMT\n  hsts: null\ndomains:\n- domain: leedsdatamill.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leedsdatamill-org/refs/heads/main/security/leedsdatamill-org-domain-security.yml
summary_line: TLSv1.3
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Open Data Portal
- United Kingdom
---
