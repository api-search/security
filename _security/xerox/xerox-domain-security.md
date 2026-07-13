---
api_specs:
- filename: xerox-public-print-openapi.yml
  format: yaml
  label: Xerox Public Print API
  slug: xerox-public-print-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xerox/refs/heads/main/openapi/xerox-public-print-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: xerox.com
  spf: true
hosts:
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: www.xerox.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: publicprintapi.services.xerox.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Xerox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xerox, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Xerox
provider_slug: xerox
slug: xerox-domain-security
source_filename: xerox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.xerox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: false\n- host: publicprintapi.services.xerox.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: xerox.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xerox/refs/heads/main/security/xerox-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Document Management
- Enterprise
- Fortune 500
- Managed Print Services
- Print Services
- Printing
---
