---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: airwisesolutions.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: airwisesolutions.app
  spf: false
hosts:
- cert_expires: Oct 23 16:16:14 2026 GMT
  host: airwisesolutions.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: developer.airwisesolutions.app
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: api.airwisesolutions.app
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Airwise Solutions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AirWise Solutions, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AirWise Solutions
provider_slug: airwise-solutions
slug: airwise-solutions-domain-security
source_filename: airwise-solutions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: airwisesolutions.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 16:16:14 2026 GMT\n  hsts: false\n- host: developer.airwisesolutions.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: false\n- host: api.airwisesolutions.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: airwisesolutions.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: airwisesolutions.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airwise-solutions/refs/heads/main/security/airwise-solutions-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Drones
- UAS
- Aviation
- Airspace
- UTM
- Public Safety
- Critical Infrastructure
- Geospatial
---
