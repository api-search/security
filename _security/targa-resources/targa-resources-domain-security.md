---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: targaresources.com
  spf: true
hosts:
- cert_expires: Sep 23 07:59:05 2026 GMT
  host: www.targaresources.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Targa Resources Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Targa Resources, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Targa Resources
provider_slug: targa-resources
slug: targa-resources-domain-security
source_filename: targa-resources-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.targaresources.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 07:59:05 2026 GMT\n  hsts: null\ndomains:\n- domain: targaresources.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/targa-resources/refs/heads/main/security/targa-resources-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Energy Infrastructure
- Fortune 500
- Midstream
- Natural Gas
- Natural Gas Liquids
- Oil And Gas
- Permian Basin
---
