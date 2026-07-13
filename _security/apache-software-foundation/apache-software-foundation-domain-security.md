---
api_specs:
- filename: apache-software-foundation-projects-api-openapi.yml
  format: yaml
  label: Apache Software Foundation Projects API
  slug: projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-software-foundation/refs/heads/main/openapi/apache-software-foundation-projects-api-openapi.yml
- filename: apache-software-foundation-whimsy-api-openapi.yml
  format: yaml
  label: Apache Software Foundation Whimsy Public Data API
  slug: whimsy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-software-foundation/refs/heads/main/openapi/apache-software-foundation-whimsy-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:root@apache.org"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apache.org
  spf: true
hosts:
- cert_expires: Aug 24 23:33:10 2026 GMT
  host: www.apache.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 23:59:59 2026 GMT
  host: projects.apache.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 11:27:01 2026 GMT
  host: whimsy.apache.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apache Software Foundation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apache Software Foundation, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Apache Software Foundation
provider_slug: apache-software-foundation
slug: apache-software-foundation-domain-security
source_filename: apache-software-foundation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.apache.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 23:33:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: projects.apache.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:59:59 2026 GMT\n  hsts: false\n- host: whimsy.apache.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 11:27:01 2026 GMT\n  hsts: false\ndomains:\n- domain: apache.org\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:root@apache.org\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-software-foundation/refs/heads/main/security/apache-software-foundation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- ASF
- Open Source
- Governance
- Projects
- Apache
---
