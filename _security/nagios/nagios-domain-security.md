---
api_specs:
- filename: nagios-xi-openapi.yml
  format: yaml
  label: Nagios XI REST API
  slug: xi-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nagios/refs/heads/main/openapi/nagios-xi-openapi.yml
- filename: ncpa-openapi.yml
  format: yaml
  label: NCPA (Nagios Cross-Platform Agent) API
  slug: ncpa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nagios/refs/heads/main/openapi/ncpa-openapi.yml
- filename: nrdp-openapi.yml
  format: yaml
  label: NRDP (Nagios Remote Data Processor) API
  slug: nrdp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nagios/refs/heads/main/openapi/nrdp-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nagios.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nagios.com
  spf: true
hosts:
- cert_expires: Oct 11 23:59:59 2026 GMT
  host: www.nagios.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 06:15:31 2026 GMT
  host: support.nagios.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nagios Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nagios, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nagios
provider_slug: nagios
slug: nagios-domain-security
source_filename: nagios-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nagios.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 23:59:59 2026 GMT\n  hsts: false\n- host: support.nagios.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 06:15:31 2026 GMT\n  hsts: false\ndomains:\n- domain: nagios.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: nagios.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nagios/refs/heads/main/security/nagios-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Monitoring
- Infrastructure Monitoring
- Network Monitoring
- Open Source
- IT Operations
- Alerting
- Observability
- Nagios XI
- Nagios Core
- NCPA
- NRPE
- NSCA
- NRDP
---
