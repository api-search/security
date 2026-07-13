---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: maggioli.cloud
  spf: true
hosts:
- cert_expires: Sep 15 12:24:22 2026 GMT
  host: www.opendata.maggioli.cloud
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opendata Maggioli Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Maggioli Cloud Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Maggioli Cloud Open Data
provider_slug: opendata-maggioli-cloud
slug: opendata-maggioli-cloud-domain-security
source_filename: opendata-maggioli-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.opendata.maggioli.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 12:24:22 2026 GMT\n  hsts: false\ndomains:\n- domain: maggioli.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opendata-maggioli-cloud/refs/heads/main/security/opendata-maggioli-cloud-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Organization
- Italy
---
