---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: genefoundry.org
  spf: false
hosts:
- cert_expires: Dec 26 06:24:21 2026 GMT
  host: genefoundry.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GeneFoundry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GeneFoundry, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: GeneFoundry
provider_slug: genefoundry-org
slug: genefoundry-org-domain-security
source_filename: genefoundry-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: genefoundry.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 06:24:21 2026 GMT\n  hsts: false\ndomains:\n- domain: genefoundry.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/genefoundry-org/security/genefoundry-org-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Biomedical
- Data
- Artificial Intelligence
- GeneFoundry
---
