---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: buildpdf.co
  spf: false
hosts:
- cert_expires: Sep  2 13:33:53 2026 GMT
  host: buildpdf.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Buildpdf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BuildPDF, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: BuildPDF
provider_slug: buildpdf
slug: buildpdf-domain-security
source_filename: buildpdf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: buildpdf.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 13:33:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: buildpdf.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buildpdf/refs/heads/main/security/buildpdf-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Documents And Productivity
- Public APIs
---
