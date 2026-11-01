---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nls.fi
  spf: true
hosts:
- cert_expires: Mar 19 11:10:23 2027 GMT
  host: www.nls.fi
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: National Land Survey Of Finland Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Land Survey of Finland, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: National Land Survey of Finland
provider_slug: national-land-survey-of-finland
slug: national-land-survey-of-finland-domain-security
source_filename: national-land-survey-of-finland-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nls.fi\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 19 11:10:23 2027 GMT\n  hsts: false\ndomains:\n- domain: nls.fi\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/national-land-survey-of-finland/security/national-land-survey-of-finland-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Geospatial Data
- Maps
- Property Register
- E‑services
- Research
---
