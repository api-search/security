---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: albumart.org
  spf: true
hosts:
- cert_expires: Dec  9 07:19:19 2026 GMT
  host: albumart.org
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Albumart Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AlbumArt.org, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: AlbumArt.org
provider_slug: albumart-org
slug: albumart-org-domain-security
source_filename: albumart-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: albumart.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 07:19:19 2026 GMT\n  hsts: null\ndomains:\n- domain: albumart.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/albumart-org/security/albumart-org-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
---
