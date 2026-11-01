---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ilmatieteenlaitos.fi
  spf: true
hosts:
- cert_expires: Mar 24 23:59:59 2027 GMT
  host: en.ilmatieteenlaitos.fi
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Finnish Meteorological Institute Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Finnish Meteorological Institute, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Finnish Meteorological Institute
provider_slug: finnish-meteorological-institute
slug: finnish-meteorological-institute-domain-security
source_filename: finnish-meteorological-institute-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: en.ilmatieteenlaitos.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 24 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ilmatieteenlaitos.fi\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/finnish-meteorological-institute/security/finnish-meteorological-institute-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Weather
- Climate
- Data
- Research
- Finland
---
