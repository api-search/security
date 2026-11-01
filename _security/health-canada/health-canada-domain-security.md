---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: canada.ca
  spf: true
hosts:
- cert_expires: Mar 11 23:59:59 2027 GMT
  host: www.canada.ca
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Health Canada Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Health Canada (Canadian Nutrient File), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Health Canada (Canadian Nutrient File)
provider_slug: health-canada
slug: health-canada-domain-security
source_filename: health-canada-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.canada.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 11 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: canada.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/health-canada/security/health-canada-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Health
- Nutrition
- Government
- Canada
---
