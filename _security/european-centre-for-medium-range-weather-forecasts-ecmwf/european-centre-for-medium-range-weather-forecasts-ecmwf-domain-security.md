---
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issuewild "digicert.com"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ecmwf.int
  spf: true
hosts:
- cert_expires: Nov 11 13:28:13 2026 GMT
  host: www.ecmwf.int
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: European Centre For Medium Range Weather Forecasts Ecmwf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for European Centre for Medium-Range Weather Forecasts (ECMWF), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: European Centre for Medium-Range Weather Forecasts (ECMWF)
provider_slug: european-centre-for-medium-range-weather-forecasts-ecmwf
slug: european-centre-for-medium-range-weather-forecasts-ecmwf-domain-security
source_filename: european-centre-for-medium-range-weather-forecasts-ecmwf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ecmwf.int\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 13:28:13 2026 GMT\n  hsts: false\ndomains:\n- domain: ecmwf.int\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/european-centre-for-medium-range-weather-forecasts-ecmwf/security/european-centre-for-medium-range-weather-forecasts-ecmwf-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Weather
- Forecasting
- Climate
- Research
- Supercomputing
- Organization
---
