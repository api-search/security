---
api_specs:
- filename: pypi-json-api-openapi.yml
  format: yaml
  label: PyPI JSON API
  slug: json
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pypi/refs/heads/main/openapi/pypi-json-api-openapi.yml
- filename: pypi-index-api-openapi.yml
  format: yaml
  label: PyPI Index API
  slug: index
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pypi/refs/heads/main/openapi/pypi-index-api-openapi.yml
- filename: pypi-integrity-api-openapi.yml
  format: yaml
  label: PyPI Integrity API
  slug: integrity
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pypi/refs/heads/main/openapi/pypi-integrity-api-openapi.yml
- filename: pypi-upload-api-openapi.yml
  format: yaml
  label: PyPI Upload API
  slug: upload
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pypi/refs/heads/main/openapi/pypi-upload-api-openapi.yml
- filename: pypi-stats-api-openapi.yml
  format: yaml
  label: PyPI Stats API
  slug: stats
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pypi/refs/heads/main/openapi/pypi-stats-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:infrastructure-staff@python.org"
  - 0 issue "amazon.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: pypi.org
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: pypistats.org
  spf: true
hosts:
- cert_expires: Oct  3 20:15:51 2026 GMT
  host: docs.pypi.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 29 04:33:07 2027 GMT
  host: pypi.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 10:39:13 2026 GMT
  host: pypistats.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pypi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PyPI, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: PyPI
provider_slug: pypi
slug: pypi-domain-security
source_filename: pypi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.pypi.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 20:15:51 2026 GMT\n  hsts: false\n- host: pypi.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 04:33:07 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: pypistats.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 10:39:13 2026 GMT\n  hsts: false\ndomains:\n- domain: pypi.org\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:infrastructure-staff@python.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: pypistats.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pypi/refs/heads/main/security/pypi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Developer Tools
- Open Source
- Package Management
- Packages
- Python
---
