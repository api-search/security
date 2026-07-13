---
api_specs:
- filename: charter-communications-spectrum-enterprise-api-openapi.yml
  format: yaml
  label: Charter Communications Spectrum Enterprise API
  slug: spectrum-enterprise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charter-communications/refs/heads/main/openapi/charter-communications-spectrum-enterprise-api-openapi.yml
- filename: charter-communications-bryte-iq-api-openapi.yml
  format: yaml
  label: Charter Communications Bryte IQ API
  slug: bryte-iq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charter-communications/refs/heads/main/openapi/charter-communications-bryte-iq-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: charter.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: spectrum.com
  spf: true
hosts:
- cert_expires: Nov 28 17:09:56 2026 GMT
  host: corporate.charter.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: enterprise.spectrum.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.charter.com
  https: false
kind: domain-security
layout: security
method: probed
name: Charter Communications Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Charter Communications, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Charter Communications
provider_slug: charter-communications
slug: charter-communications-domain-security
source_filename: charter-communications-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: corporate.charter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 17:09:56 2026 GMT\n  hsts: false\n- host: enterprise.spectrum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: null\n- host: api.charter.com\n  https: false\ndomains:\n- domain: charter.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: spectrum.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/charter-communications/refs/heads/main/security/charter-communications-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Broadband
- Cable
- CAMARA
- Enterprise
- Network as a Service
- NaaS
- Spectrum
- Telecommunications
- Ticketing
- Fortune 500
---
