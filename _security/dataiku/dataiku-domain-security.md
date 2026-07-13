---
api_specs:
- filename: index.html
  format: yaml
  label: Dataiku Public API
  slug: dataiku-public-api
  spec_type: OpenAPI
  url: https://doc.dataiku.com/dss/latest/publicapi/rest/index.html
- filename: dataiku-api-node-admin-openapi.yml
  format: yaml
  label: Dataiku API Node Administration API
  slug: dataiku-api-node-administration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dataiku/refs/heads/main/openapi/dataiku-api-node-admin-openapi.yml
- filename: dataiku-govern-api-openapi.yml
  format: yaml
  label: Dataiku Govern API
  slug: dataiku-govern-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dataiku/refs/heads/main/openapi/dataiku-govern-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dataiku.com
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:infrastructure-staff@python.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: pypi.org
  spf: true
hosts:
- cert_expires: Sep  5 15:20:49 2026 GMT
  host: developer.dataiku.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 00:27:39 2026 GMT
  host: www.dataiku.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 29 04:33:07 2027 GMT
  host: pypi.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dataiku Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dataiku, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dataiku
provider_slug: dataiku
slug: dataiku-domain-security
source_filename: dataiku-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.dataiku.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 15:20:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.dataiku.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 00:27:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: pypi.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 04:33:07 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dataiku.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: pypi.org\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:infrastructure-staff@python.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dataiku/refs/heads/main/security/dataiku-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Analytics
- Artificial Intelligence
- Data Platform
- Data Science
- Machine Learning
---
