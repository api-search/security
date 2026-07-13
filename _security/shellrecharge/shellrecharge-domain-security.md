---
api_specs:
- filename: shellrecharge-openapi.yml
  format: yaml
  label: ShellRecharge EV Public Locations API
  slug: shellrecharge-public-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shellrecharge/refs/heads/main/openapi/shellrecharge-openapi.yml
- filename: shellrecharge-openapi.yml
  format: yaml
  label: ShellRecharge EV Public Charge Sessions API
  slug: shellrecharge-public-charge-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shellrecharge/refs/heads/main/openapi/shellrecharge-openapi.yml
- filename: shellrecharge-openapi.yml
  format: yaml
  label: ShellRecharge OCPI API
  slug: shellrecharge-ocpi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shellrecharge/refs/heads/main/openapi/shellrecharge-openapi.yml
- filename: shellrecharge-openapi.yml
  format: yaml
  label: ShellRecharge Tariffs API
  slug: shellrecharge-tariffs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shellrecharge/refs/heads/main/openapi/shellrecharge-openapi.yml
- filename: shellrecharge-openapi.yml
  format: yaml
  label: ShellRecharge Tokens API
  slug: shellrecharge-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shellrecharge/refs/heads/main/openapi/shellrecharge-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: shellrecharge.com
  spf: true
- caa:
  - 0 iodef "mailto:ipladmin@shell.com"
  - 0 issue "godaddy.com"
  - 0 issue "globalsign.com"
  - 0 issue "entrust.net"
  - 0 issue "symantec.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: shell.com
  spf: true
hosts:
- cert_expires: Sep 26 07:12:25 2026 GMT
  host: shellrecharge.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: developer.shell.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: api.shell.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Shellrecharge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ShellRecharge, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: ShellRecharge
provider_slug: shellrecharge
slug: shellrecharge-domain-security
source_filename: shellrecharge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shellrecharge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 07:12:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.shell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: api.shell.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: shellrecharge.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: shell.com\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:ipladmin@shell.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"symantec.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shellrecharge/refs/heads/main/security/shellrecharge-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- EV Charging
- Electric Vehicles
- Mobility
- Charge Points
- OCPI
- Energy
---
