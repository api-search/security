---
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:ukdsalerts@essex.ac.uk"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ukdataservice.ac.uk
  spf: true
hosts:
- cert_expires: Nov 15 10:45:57 2026 GMT
  host: ukdataservice.ac.uk
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Uk Data Service Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UK Data Service, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: UK Data Service
provider_slug: uk-data-service
slug: uk-data-service-domain-security
source_filename: uk-data-service-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ukdataservice.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 10:45:57 2026 GMT\n  hsts: false\ndomains:\n- domain: ukdataservice.ac.uk\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:ukdsalerts@essex.ac.uk\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uk-data-service/refs/heads/main/security/uk-data-service-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Data
- Research
- Education
- United Kingdom
---
