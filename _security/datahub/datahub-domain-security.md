---
api_specs:
- filename: datahub-openapi-openapi.yml
  format: yaml
  label: DataHub OpenAPI
  slug: datahub-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datahub/refs/heads/main/openapi/datahub-openapi-openapi.yml
- filename: datahub-actions-asyncapi.yml
  format: yaml
  label: DataHub Actions Framework
  slug: datahub-actions-framework
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/datahub/refs/heads/main/asyncapi/datahub-actions-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: datahub.com
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
- cert_expires: Sep 16 18:54:21 2026 GMT
  host: datahub.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 21:27:55 2026 GMT
  host: docs.datahub.com
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
name: Datahub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DataHub, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DataHub
provider_slug: datahub
slug: datahub-domain-security
source_filename: datahub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datahub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 18:54:21 2026 GMT\n  hsts: false\n- host: docs.datahub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 21:27:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: pypi.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 04:33:07 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: datahub.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: pypi.org\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:infrastructure-staff@python.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datahub/refs/heads/main/security/datahub-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Data Catalog
- Data Discovery
- Data Governance
- Data Lineage
- Metadata
---
