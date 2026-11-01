---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: geosa.gov.sa
  spf: true
hosts:
- cert_expires: Feb 21 23:59:59 2027 GMT
  host: geosa.gov.sa
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: General Authority For Survey And Geospatial Information Geosa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for General Authority for Survey and Geospatial Information (GEOSA), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: General Authority for Survey and Geospatial Information (GEOSA)
provider_slug: general-authority-for-survey-and-geospatial-information-geosa
slug: general-authority-for-survey-and-geospatial-information-geosa-domain-security
source_filename: general-authority-for-survey-and-geospatial-information-geosa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: geosa.gov.sa\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 21 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: geosa.gov.sa\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/general-authority-for-survey-and-geospatial-information-geosa/security/general-authority-for-survey-and-geospatial-information-geosa-domain-security.yml
summary_line: TLSv1.2 · DNSSEC · DMARC
tags:
- Company
- Government
- Geospatial
- Surveying
- Saudi-Arabia
---
