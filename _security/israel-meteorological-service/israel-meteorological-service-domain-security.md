---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ims.gov.il
  spf: true
hosts:
- cert_expires: Nov 25 23:59:59 2026 GMT
  host: ims.gov.il
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Israel Meteorological Service Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IMS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: IMS
provider_slug: israel-meteorological-service
slug: israel-meteorological-service-domain-security
source_filename: israel-meteorological-service-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ims.gov.il\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 25 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: ims.gov.il\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/israel-meteorological-service/security/israel-meteorological-service-domain-security.yml
summary_line: TLSv1.2 · DNSSEC · DMARC
tags:
- meteorology
- weather
- Israel
- government
- public-service
---
