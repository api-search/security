---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: hrsa.gov
  spf: true
hosts:
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: www.hrsa.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 19:15:06 2026 GMT
  host: data.hrsa.gov
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Health Resources And Services Administration Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Health Resources and Services Administration, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Health Resources and Services Administration
provider_slug: health-resources-and-services-administration
slug: health-resources-and-services-administration-domain-security
source_filename: health-resources-and-services-administration-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hrsa.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: null\n- host: data.hrsa.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 19:15:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hrsa.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/health-resources-and-services-administration/refs/heads/main/security/health-resources-and-services-administration-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
- Healthcare
- Open Data
- Public Health
---
