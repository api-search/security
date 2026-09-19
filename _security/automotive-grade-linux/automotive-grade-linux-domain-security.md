---
api_specs:
- filename: automotive-grade-linux-categories-api-openapi.yml
  format: yaml
  label: Automotive Grade Linux Categories API
  slug: automotive-grade-linux-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automotive-grade-linux/refs/heads/main/openapi/automotive-grade-linux-categories-api-openapi.yml
- filename: automotive-grade-linux-common-api-openapi.yml
  format: yaml
  label: Automotive Grade Linux Common API
  slug: automotive-grade-linux-common-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automotive-grade-linux/refs/heads/main/openapi/automotive-grade-linux-common-api-openapi.yml
- filename: automotive-grade-linux-doc-api-openapi.yml
  format: yaml
  label: Automotive Grade Linux Doc API
  slug: automotive-grade-linux-doc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automotive-grade-linux/refs/heads/main/openapi/automotive-grade-linux-doc-api-openapi.yml
- filename: automotive-grade-linux-events-api-openapi.yml
  format: yaml
  label: Automotive Grade Linux Events API
  slug: automotive-grade-linux-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automotive-grade-linux/refs/heads/main/openapi/automotive-grade-linux-events-api-openapi.yml
- filename: automotive-grade-linux-events-pro-api-openapi.yml
  format: yaml
  label: Automotive Grade Linux Events Pro API
  slug: automotive-grade-linux-events-pro-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automotive-grade-linux/refs/heads/main/openapi/automotive-grade-linux-events-pro-api-openapi.yml
- filename: automotive-grade-linux-organizers-api-openapi.yml
  format: yaml
  label: Automotive Grade Linux Organizers API
  slug: automotive-grade-linux-organizers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automotive-grade-linux/refs/heads/main/openapi/automotive-grade-linux-organizers-api-openapi.yml
- filename: automotive-grade-linux-tags-api-openapi.yml
  format: yaml
  label: Automotive Grade Linux Tags API
  slug: automotive-grade-linux-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automotive-grade-linux/refs/heads/main/openapi/automotive-grade-linux-tags-api-openapi.yml
- filename: automotive-grade-linux-venues-api-openapi.yml
  format: yaml
  label: Automotive Grade Linux Venues API
  slug: automotive-grade-linux-venues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automotive-grade-linux/refs/heads/main/openapi/automotive-grade-linux-venues-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: automotivelinux.org
  spf: true
hosts:
- cert_expires: Nov  5 17:59:39 2026 GMT
  host: www.automotivelinux.org
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 09:46:33 2026 GMT
  host: docs.automotivelinux.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 27 17:07:36 2026 GMT
  host: lava.automotivelinux.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Automotive Grade Linux Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Automotive Grade Linux, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Automotive Grade Linux
provider_slug: automotive-grade-linux
slug: automotive-grade-linux-domain-security
source_filename: automotive-grade-linux-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.automotivelinux.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 17:59:39 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: docs.automotivelinux.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 09:46:33 2026 GMT\n  hsts: false\n- host: lava.automotivelinux.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 17:07:36 2026 GMT\n  hsts: false\ndomains:\n- domain: automotivelinux.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/automotive-grade-linux/refs/heads/main/security/automotive-grade-linux-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automotive
- Connected Vehicles
- Embedded Linux
- In-Vehicle Infotainment
- IoT
- Linux Foundation
- Open-Source
- Software Defined Vehicles
---
