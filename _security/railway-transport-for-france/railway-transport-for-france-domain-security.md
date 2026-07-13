---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sncf.com
  spf: true
hosts:
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: www.digital.sncf.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Railway Transport For France Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Railway Transport for France, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Railway Transport for France
provider_slug: railway-transport-for-france
slug: railway-transport-for-france-domain-security
source_filename: railway-transport-for-france-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.digital.sncf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: sncf.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/railway-transport-for-france/refs/heads/main/security/railway-transport-for-france-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Transportation
- Public APIs
---
