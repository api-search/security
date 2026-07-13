---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: amerigeoss.org
  spf: true
hosts:
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: data.amerigeoss.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Data Amerigeoss Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AmeriGEOSS Community Platform, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AmeriGEOSS Community Platform
provider_slug: data-amerigeoss-org
slug: data-amerigeoss-org-domain-security
source_filename: data-amerigeoss-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.amerigeoss.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: amerigeoss.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/data-amerigeoss-org/refs/heads/main/security/data-amerigeoss-org-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Organization
- United States
---
