---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fca.gov
  spf: true
hosts:
- cert_expires: Nov  1 23:59:59 2026 GMT
  host: www.fca.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Farm Credit Administration Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Farm Credit Administration, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Farm Credit Administration
provider_slug: farm-credit-administration
slug: farm-credit-administration-domain-security
source_filename: farm-credit-administration-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fca.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: fca.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/farm-credit-administration/refs/heads/main/security/farm-credit-administration-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Agriculture
- Farms
- Federal Government
- Finance
- Regulation
---
