---
api_specs:
- filename: nagios-config-api-openapi.yml
  format: yaml
  label: Nagios Config API
  slug: nagios-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nagios/refs/heads/main/openapi/nagios-config-api-openapi.yml
- filename: nagios-cpu-api-openapi.yml
  format: yaml
  label: Nagios CPU API
  slug: nagios-cpu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nagios/refs/heads/main/openapi/nagios-cpu-api-openapi.yml
- filename: nagios-disk-api-openapi.yml
  format: yaml
  label: Nagios Disk API
  slug: nagios-disk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nagios/refs/heads/main/openapi/nagios-disk-api-openapi.yml
- filename: nagios-interface-api-openapi.yml
  format: yaml
  label: Nagios Interface API
  slug: nagios-interface-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nagios/refs/heads/main/openapi/nagios-interface-api-openapi.yml
- filename: nagios-memory-api-openapi.yml
  format: yaml
  label: Nagios Memory API
  slug: nagios-memory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nagios/refs/heads/main/openapi/nagios-memory-api-openapi.yml
- filename: nagios-objects-api-openapi.yml
  format: yaml
  label: Nagios Objects API
  slug: nagios-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nagios/refs/heads/main/openapi/nagios-objects-api-openapi.yml
- filename: nagios-plugins-api-openapi.yml
  format: yaml
  label: Nagios Plugins API
  slug: nagios-plugins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nagios/refs/heads/main/openapi/nagios-plugins-api-openapi.yml
- filename: nagios-processes-api-openapi.yml
  format: yaml
  label: Nagios Processes API
  slug: nagios-processes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nagios/refs/heads/main/openapi/nagios-processes-api-openapi.yml
- filename: nagios-services-api-openapi.yml
  format: yaml
  label: Nagios Services API
  slug: nagios-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nagios/refs/heads/main/openapi/nagios-services-api-openapi.yml
- filename: nagios-submission-api-openapi.yml
  format: yaml
  label: Nagios Submission API
  slug: nagios-submission-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nagios/refs/heads/main/openapi/nagios-submission-api-openapi.yml
- filename: nagios-system-api-openapi.yml
  format: yaml
  label: Nagios System API
  slug: nagios-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nagios/refs/heads/main/openapi/nagios-system-api-openapi.yml
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
