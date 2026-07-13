---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: devitjobs.uk
  spf: true
hosts:
- cert_expires: Oct  6 16:58:43 2026 GMT
  host: devitjobs.uk
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Devitjobs Uk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DevITjobs UK, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: DevITjobs UK
provider_slug: devitjobs-uk
slug: devitjobs-uk-domain-security
source_filename: devitjobs-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: devitjobs.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 16:58:43 2026 GMT\n  hsts: false\ndomains:\n- domain: devitjobs.uk\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/devitjobs-uk/refs/heads/main/security/devitjobs-uk-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Jobs
- Public APIs
---
