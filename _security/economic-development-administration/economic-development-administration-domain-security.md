---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: eda.gov
  spf: true
hosts:
- cert_expires: Sep 18 18:15:08 2026 GMT
  host: www.eda.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Economic Development Administration Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Economic Development Administration, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Economic Development Administration
provider_slug: economic-development-administration
slug: economic-development-administration-domain-security
source_filename: economic-development-administration-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eda.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 18:15:08 2026 GMT\n  hsts: null\ndomains:\n- domain: eda.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/economic-development-administration/refs/heads/main/security/economic-development-administration-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Economic Development
- Federal Government
---
