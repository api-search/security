---
api_specs:
- filename: shutterstock-openapi.yml
  format: yaml
  label: Shutterstock API
  slug: shutterstock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shutterstock/refs/heads/main/openapi/shutterstock-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: shutterstock.com
  spf: true
hosts:
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: www.shutterstock.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: api.shutterstock.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Shutterstock Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shutterstock, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Shutterstock
provider_slug: shutterstock
slug: shutterstock-domain-security
source_filename: shutterstock-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.shutterstock.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: null\n- host: api.shutterstock.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: shutterstock.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shutterstock/refs/heads/main/security/shutterstock-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Images
- Media
- Photos
- Stock Images
- Videos
- Audio
- Licensing
- Creative Content
---
