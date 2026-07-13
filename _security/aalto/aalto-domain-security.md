---
api_specs:
- filename: api
  format: yaml
  label: Aaltodoc Repository (OAI-PMH and REST)
  slug: aaltodoc-oai
  spec_type: OpenAPI
  url: https://aaltodoc.aalto.fi/server/api
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aalto.fi
  spf: true
hosts:
- cert_expires: Jan 12 11:22:25 2027 GMT
  host: www.aalto.fi
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 12 14:20:03 2026 GMT
  host: 3scale.apps.ocp4.aalto.fi
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 10:44:56 2026 GMT
  host: data.aalto.fi
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aalto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aalto University, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Aalto University
provider_slug: aalto
slug: aalto-domain-security
source_filename: aalto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aalto.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 11:22:25 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: 3scale.apps.ocp4.aalto.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 14:20:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: data.aalto.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 10:44:56 2026 GMT\n  hsts: false\ndomains:\n- domain: aalto.fi\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aalto/refs/heads/main/security/aalto-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- Linked Data
- Finland
---
